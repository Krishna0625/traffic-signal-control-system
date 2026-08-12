pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Downloading code from GitHub'
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo 'Building Traffic Signal Control System'
            }
        }

        stage('Test') {
            steps {
                echo 'Testing Traffic Signal Control System'
                sh 'ls -la'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deployment Successful'
            }
        }
    }

    post {
        success {
            echo 'Pipeline Executed Successfully'
        }

        failure {
            echo 'Pipeline Failed'
        }
    }
}