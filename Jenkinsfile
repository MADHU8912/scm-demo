pipeline {
    agent any

    stages {

        stage('Checkout SCM') {
            steps {
                echo 'Fetching code from GitHub'
            }
        }

        stage('Check Files') {
            steps {
                bat 'dir'
            }
        }

        stage('Build') {
            steps {
                bat 'echo Building project...'
            }
        }

        stage('Test') {
            steps {
                bat 'echo Running tests...'
            }
        }

        stage('Deploy') {
            steps {
                bat 'echo Deploying project...'
            }
        }

        stage('Build Report') {
            steps {
                bat 'echo Build + Test + Deploy SUCCESS > build-report.txt'
                bat 'type build-report.txt'
            }
        }
    }

    post {
        success {
            echo 'Pipeline completed successfully'
        }
        failure {
            echo 'Pipeline failed'
        }
    }
}
