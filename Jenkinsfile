pipeline {
    agent any
    
    stages {
        stage('Hello World') {
            steps {
                
                bat 'javac HelloWorld.java'
                bat 'java HelloWorld.java'
            }
        }
        stage('Hello Wipro') {
            steps {
                
                bat 'javac HelloWipro.java'
                bat 'java HelloWipro.java'
            }
        }
        stage('Hello Jenkins') {
            steps {
         
                bat 'javac HelloJenkins.java'
                bat 'java HelloJenkins.java'
            }
        }
    }
    
    post {
        always {
            
            echo 'Pipeline completed'
           
        }
    }
}
