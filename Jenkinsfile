pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                echo "Pulling code from GitHub..."
            }
        }

        stage('Install Dependencies') {
            steps {
                echo "Installing project dependencies..."
            }
        }

        stage('Build') {
            steps {
                echo "Building the application..."
            }
        }

        stage('Test') {
            steps {
                echo "Running tests..."
            }
        }
    }

    post {
        always {
            echo "Pipeline run completed."
        }
    }
}
