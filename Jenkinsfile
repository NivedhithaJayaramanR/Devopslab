pipeline {
    agent any

    stages {
        stage('Checkout Code') {
            steps {
                git branch: 'main', url: 'https://github.com/NivedhithaJayaramanR/Devopslab.git'
            }
        }

        stage('Build Backend') {
            steps {
                echo 'Building backend...'
                // Example: mvn clean install
            }
        }

        stage('Build Frontend') {
            steps {
                echo 'Building frontend...'
                // Example: npm install && npm run build
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application...'
            }
        }
    }

    post {
        success {
            echo '✅ Build successful!'
        }
        failure {
            echo '❌ Build failed. Check logs.'
        }
    }
}
