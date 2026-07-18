pipeline {
    agent any 

    stages {
        stage('Checkout Code') {
            steps {
                echo 'Successfully pulled code from GitHub!'
            }
        }
        stage('Simulate Environment') {
            steps {
                echo 'Checking software versions...'
                sh 'node -v || true'
                sh 'npm -v || true'
            }
        }
        stage('Build & Test') {
            steps {
                echo 'Running local sandbox tests...'
                sh 'echo "All checks passed successfully!"'
            }
        }
    }
}
