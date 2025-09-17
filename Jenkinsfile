pipeline {
    agent any   // run on any available Jenkins agent/node

    stages {
        stage('Checkout') {
            steps {
                // Jenkins automatically checks out the branch for multibranch pipeline,
                // but you can be explicit:
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo 'Building the project...'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deployment step (dummy)...'
            }
        }
    }

    post {
        always {
            echo 'Pipeline completed.'
        }
    }
}
