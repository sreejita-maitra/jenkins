pipeline {
    agent any
    
    stages {
        stage('Hello World') {
            steps {
                sh 'javac HelloWorld.java'
                sh 'java HelloWorld.java'
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
             
        }
    }
}
