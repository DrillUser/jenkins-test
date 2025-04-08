pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'echo "Hello, Jenkins!"'
            }
        }
        stage('Test') {
            steps {
                sh 'echo "Running tests..."'
                sh 'sleep 5'
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
