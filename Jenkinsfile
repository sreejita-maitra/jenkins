pipeline {
    agent any
    
    stages {
        stage('Hello World') {
            steps {
                echo 'Hello World'
            }
        }
        stage('Hello Wipro') {
            steps {
                echo 'Hello Wipro'
            }
        }
        stage('Hello Jenkins') {
            steps {
                echo 'Hello Jenkins'
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
