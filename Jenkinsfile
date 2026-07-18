pipeline {
    agent any 

    stages {
        stage('Test Everything') {
            steps {
                echo "Running standard linting and tests on branch: ${env.BRANCH_NAME}"
                sh 'echo "Tests passed!"'
            }
        }

        stage('Deploy to Staging') {
            when {
                branch 'develop'
            }
            steps {
                echo 'Simulating deployment to the STAGING environment...'
            }
        }

        stage('Deploy to Production') {
            when {
                branch 'main' // or 'production' depending on what your primary branch is named
            }
            steps {
                echo '🚀 Simulating deployment to the PRODUCTION environment!!!'
            }
        }
    }
}
