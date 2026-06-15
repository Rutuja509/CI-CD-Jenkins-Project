pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git 'https://github.com/Rutuja509/CI-CD-Jenkins-Project.git'
            }
        }

        stage('Install') {
            steps {
                sh 'pip install -r requirements.txt'
            }
        }

        stage('Test') {
            steps {
                sh 'pytest'
            }
        }

        stage('Run Application') {
            steps {
                sh 'python app.py'
            }
        }
    }
}