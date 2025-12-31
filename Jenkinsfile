pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo "Building application"
                sh 'chmod +x test-app.sh'
            }
        }

        stage('Test') {
            steps {
                echo "Running tests"
                sh './test-app.sh'
            }
        }

        stage('Deploy') {
            steps {
                echo "Deploying application"
            }
        }
    }
}
