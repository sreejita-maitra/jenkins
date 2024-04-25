pipeline {
    agent any
    
    stages {
        stage('Hello World') {
            steps {
                script {
                    try {
                        sh 'javac HelloWorld.java'
                        sh 'java HelloWorld'
                    } catch (Exception e) {
                        echo "Failed to compile or execute HelloWorld: ${e.message}"
                        currentBuild.result = 'FAILURE'
                    }
                }
            }
        }
        // Repeat similar steps for other stages
    }
    
    post {
        always {
            echo 'Pipeline completed'
        }
    }
}
