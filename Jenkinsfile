pipeline {
    agent any

    stages {
        stage('Build Report') {
            steps {
                bat 'echo Jenkins pipeline is working > build-report.txt'
                bat 'type build-report.txt'
            }
        }
    }
}
