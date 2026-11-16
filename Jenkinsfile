
pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                echo "Branch: ${env.BRANCH_NAME}"
                echo 'Source code checked out'
            }
        }

        stage('Build') {
            steps {
                echo "Building ${env.BRANCH_NAME}"
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests'
            }
        }
    }

    post {
        success {
            echo 'Pipeline successful!'
        }
    }
}
