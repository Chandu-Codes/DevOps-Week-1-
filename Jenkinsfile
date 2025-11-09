pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building the project...'
                bat 'echo Compiling source code...'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                bat 'echo Running automated tests...'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application...'
                bat 'echo Deploying build...'
            }
        }
    }

    post {
        success {
            echo '✅ Build completed successfully!'
        }
        failure {
            echo '❌ Build failed. Check logs for details.'
        }
    }
}
