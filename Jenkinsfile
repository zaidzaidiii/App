pipeline {
    agent any

    stages {
        stage('Checkout Code') {
            steps {
                echo "📥 Fetching code from GitHub..."
            }
        }
        stage('Verify Files') {
            steps {
                echo "🔍 Checking repo contents on remote server..."
                // Check if index.html exists in workspace
                sh 'ls -la'
                sh 'test -f index.html && echo "HTML file found!"'
            }
        }
    }
}