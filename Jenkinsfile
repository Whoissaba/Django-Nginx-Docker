pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                // Checkout the code from GitHub
                git 'https://github.com/Whoissaba/Django-Nginx-Docker.git'
            }
        }
        
        stage('Build') {
            steps {
                // Add your build steps here
                // For example, if it's a Docker project, you might build the Docker image
                script {
                    sh 'docker build -t your-image-name .'
                }
            }
        }
        
        // Add more stages for testing, deployment, etc. as needed
    }
    
    post {
        success {
            echo 'Build succeeded! You can add further actions here.'
        }
        failure {
            echo 'Build failed! You can add further actions for failure handling here.'
        }
    }
}
