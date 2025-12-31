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
                sh 'chmod +x app.sh'
            }
        }

        stage('Test') {
            steps {
                echo "Running tests"
                sh './app.sh'
            }
        }

        stage('Deploy') {
            steps {
                echo "Deploying application"
            }
        }
    }
}
