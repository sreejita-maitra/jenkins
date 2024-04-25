pipeline {
    agent any
    
    stages {
        stage('Hello World') {
            steps {
                sh 'java HelloWorld'
            }
        }
        stage('Hello Wipro') {
            steps {
                sh 'java HelloWipro'
            }
        }
        stage('Hello Jenkins') {
            steps {
                sh 'java HelloJenkins'
            }
        }
    }
    
    post {
        always {
            // Archive artifacts
            archiveArtifacts artifacts: '**/target/*.jar', fingerprint: true
            
            // Send email notification
            emailext (
                to: 'sreejita.maitra@gmail.com',
                subject: 'Pipeline Status - ${currentBuild.result}',
                body: 'The pipeline execution status is ${currentBuild.result}',
                attachLog: true
            )
        }
    }
}
