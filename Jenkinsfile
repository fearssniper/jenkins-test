pipeline {
    agent any

    environment {
        REPO_URL = 'https://github.com/yourusername/your-repo.git'
        BRANCH = 'main'
    }

    stages {
        stage('Checkout') {
            steps {
                git branch: "${BRANCH}", url: "${REPO_URL}"
            }
        }
        stage('Build') {
            steps {
                echo 'Building...'
                // Add build steps here
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
                sh 'python3 -m unittest discover'
            }
        }
    }
}
