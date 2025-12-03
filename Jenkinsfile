pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                echo "Pulling code from GitHub..."
                checkout scm
            }
        }

        stage('Install Dependencies') {
            steps {
                echo "Installing project dependencies..."
                sh 'npm install'
            }
        }

        stage('Build') {
            steps {
                echo "Building the application..."
                sh 'npm run build'
            }
        }

        stage('Test') {
            steps {
                echo "Running tests..."
                sh 'npm test'
            }
        }
    }

    post {
        always {
            echo "Pipeline run completed."
        }
    }
}
