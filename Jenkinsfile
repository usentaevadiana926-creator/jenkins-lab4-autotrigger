pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo "Source code checkout completed"
            }
        }

        stage('Commit Information') {
            steps {
                echo "Branch: ${env.BRANCH_NAME}"
                echo "Build number: ${env.BUILD_NUMBER}"
            }
        }

        stage('Build') {
            steps {
                echo "Building project..."
            }
        }

        stage('Test') {
            steps {
                echo "Running tests..."
            }
        }
    }

    post {
        success {
            echo "Pipeline completed successfully"
        }

        failure {
            echo "Pipeline failed. Check Console Output"
        }
    }
}
