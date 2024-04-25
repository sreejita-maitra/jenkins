pipeline {
    agent any
    
    stages {
        stage('Hello World') {
            steps {
                // Compile and run HelloWorld Java program using batch commands
                bat 'javac HelloWorld.java'
                bat 'java HelloWorld.java'
            }
        }
        stage('Hello Wipro') {
            steps {
                // Compile and run HelloWipro Java program using batch commands
                bat 'javac HelloWipro.java'
                bat 'java HelloWipro.java'
            }
        }
        stage('Hello Jenkins') {
            steps {
                // Compile and run HelloJenkins Java program using batch commands
                bat 'javac HelloJenkins.java'
                bat 'java HelloJenkins.java'
            }
        }
    }
    
    post {
        always {
            // Add post-build actions here
            echo 'Pipeline completed'
            
            // You can add more post-build actions such as sending notifications, archiving artifacts, etc.
            // For example:
            archiveArtifacts artifacts: '**/target/*.jar', fingerprint: true
            mail to: 'sreejita.maitra@wipro.com', subject: 'Pipeline completed', body: 'The Jenkins pipeline has completed successfully.'
        }
    }
}
