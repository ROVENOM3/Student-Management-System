pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/ROVENOM3/Student-Management-System'
            }
        }

        stage('Test') {
            steps {
                echo 'Testing Student Management System...'
                bat 'dir'
            }
        }

        stage('Build') {
            steps {
                echo 'Student Management System build successful!'
            }
        }
    }

    post {
        success {
            echo 'CI Pipeline Successful!'
        }

        failure {
            echo 'CI Pipeline Failed!'
        }
    }
}