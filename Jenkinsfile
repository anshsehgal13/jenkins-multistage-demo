pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo "🔧 Building app for branch: ${env.BRANCH_NAME}"
                sh 'echo Building...'
                sh 'sleep 2'
            }
        }

        stage('Test') {
            when {
                branch 'dev'
            }
            steps {
                echo "🧪 Running tests for branch: ${env.BRANCH_NAME}"
                sh 'echo Testing...'
                sh 'sleep 2'
            }
        }

        stage('Deploy') {
            when {
                branch 'main'
            }
            steps {
                echo "🚀 Deploying for branch: ${env.BRANCH_NAME}"
                sh 'echo Deploying...'
                sh 'sleep 2'
            }
        }
    }

    post {
        success {
            echo "✅ Pipeline completed for branch: ${env.BRANCH_NAME}"
        }
    }
}
