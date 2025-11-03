pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo '🔧 Building the inventory-api app...'
                sh 'echo "Building application..."'
                sh 'sleep 2'
            }
        }

        stage('Test') {
            steps {
                echo '🧪 Running tests...'
                sh 'echo "Running basic tests..."'
                sh 'sleep 2'
            }
        }

        stage('Deploy') {
            steps {
                echo '🚀 Deploying application...'
                sh 'echo "Deploying to environment..."'
                sh 'sleep 2'
            }
        }
    }

    post {
        success {
            echo '✅ Pipeline completed successfully!'
        }
        failure {
            echo '❌ Pipeline failed!'
        }
    }
}
