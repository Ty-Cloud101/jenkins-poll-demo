pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Checking out source code...'
                // The 'checkout scm' step will be automatically used by the pipeline
                // when it's pulled from the repository.
            }
        }
        stage('Build') {
            steps {
                echo 'Building the application...'
                // Add your build commands here, e.g., sh 'make'
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests...'
                // Add your test commands here, e.g., sh 'make test'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying application...'
                // Add your deployment commands here
            }
        }
    }

    post {
        always {
            echo 'This will always run.'
        }
        success {
            echo 'Pipeline succeeded!'
        }
        failure {
            echo 'Pipeline failed.'
        }
    }
}
