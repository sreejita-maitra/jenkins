pipeline {
    agent any
    
    stages {
        stage('Hello World') {
            steps {
                // Compile and run Hello World Java program
                sh 'javac HelloWorld.java'
                sh 'java HelloWorld.java'
            }
        }
        stage('Hello Wipro') {
            steps {
                // Compile and run Hello Wipro Java program
                sh 'javac HelloWipro.java'
                sh 'java HelloWipro.java'
            }
        }
        stage('Hello Jenkins') {
            steps {
                // Compile and run Hello Jenkins Java program
                sh 'javac HelloJenkins.java'
                sh 'java HelloJenkins.java'
            }
        }
    }
    
    post {
        always {
            // Add post-build actions here
            echo 'Pipeline completed'
        }
    }
}
