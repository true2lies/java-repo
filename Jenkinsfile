pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                // Add your build steps here
                echo 'Building the project...'
            }
        }

        stage('Test') {
            steps {
                // Add your test steps here
                echo 'Running tests...'
            }
        }

        stage('Deploy') {
            steps {
                // Add your deployment steps here
                echo 'Deploying the application...'
            }
        }
    }

    post {
        always {
            // Send an email with the build results
            emailext(
                body: 'The pipeline has completed. Check the build logs for more details.',
                subject: 'Pipeline Completed',
                to: 'true2lies36@gmail.com'
            )
        }
    }
}
