pipeline {
    agent any

    stages {
        stage('Checkout Code') {
            steps {
                echo "📥 Fetching latest code from GitHub..."
            }
        }
        stage('Deploy Live to Nginx') {
            steps {
                echo "🚀 Deploying index.html to Nginx web root..."
                # index.html ko nginx ke live path par copy kar rahe hain
                sh 'sudo cp index.html /var/www/html/index.html'
            }
        }
    }
}
