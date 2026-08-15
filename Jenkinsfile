pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/YOUR_USERNAME/student-management-system.git'
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