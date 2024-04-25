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
            // Post-build actions, if any
        }
    }
}
