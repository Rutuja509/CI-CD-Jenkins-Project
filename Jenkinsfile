pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git branch: 'master',
                    url: 'https://github.com/Rutuja509/Scripting.git'
            }
        }

        stage('Build') {
            steps {
                echo 'Build completed successfully'
            }
        }

        stage('Test') {
            steps {
                echo 'Test completed successfully'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deployment completed successfully'
            }
        }
    }

    post {
        success {
            echo 'Pipeline completed successfully'
        }
        failure {
            echo 'Pipeline failed'
        }
    }
}