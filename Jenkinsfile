pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/DrillUser/jenkins-test.git'
            }
        }
        stage('Build') {
            steps {
                sh 'echo "Hello, Jenkins!"'
            }
        }
        stage('Test') {
            steps {
                sh 'echo "Running tests..."'
                sh 'sleep 5'  // Имитация тестов
            }
        }
        stage('Deploy') {
            steps {
                sh 'echo "Deploying to production..."'
            }
        }
    }
    post {
        always {
            echo 'Pipeline finished!'
        }
    }
}
