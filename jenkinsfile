pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Checking out the repository...'
                git branch: 'main', url: 'https://github.com/Lavana2004/Landing-page.git'
            }
        }

        stage('Install Dependencies') {
            steps {
                echo 'No dependencies to install for a static website.'
                // Placeholder for future dependency installation commands
                // Example: sh 'npm install'
            }
        }

        stage('Run Tests') {
            steps {
                echo 'No tests defined yet.'
                // Placeholder for future test commands
                // Example: sh 'npm test'
            }
        }

        stage('Publish Test Results') {
            steps {
                echo 'No test results to publish.'
                // Placeholder for publishing test results
                // Example: junit 'test-results.xml'
            }
        }
    }

    post {
        always {
            echo 'Cleaning up workspace...'
            cleanWs() // Cleans up the workspace after the pipeline run
        }
        success {
            echo 'Pipeline completed successfully!'
        }
        failure {
            echo 'Pipeline failed. Please check the logs.'
        }
    }
}
