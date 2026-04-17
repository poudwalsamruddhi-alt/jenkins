pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/your-repo.git'
            }
        }

        stage('Build') {
            steps {
                sh 'echo Build step'
            }
        }

        stage('Test') {
            steps {
                sh 'echo Test step'
            }
        }

        stage('Deploy') {
            steps {
                sh 'echo Deploy step'
            }
        }
    }
}
