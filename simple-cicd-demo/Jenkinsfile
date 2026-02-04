pipeline {
    agent any

    stages {
        stage('Checkout Code') {
            steps {
                echo 'Code already checked out by Jenkins'
            }
        }

        stage('List Files') {
            steps {
                bat 'dir'
                bat 'dir site'
            }
        }

        stage('Show HTML Content') {
            steps {
                bat 'type site\\index.html'
            }
        }
    }

    post {
        success {
            echo 'Pipeline ran successfully ✅'
        }
        failure {
            echo 'Pipeline failed ❌'
        }
    }
}
