pipeline {
    agent {
        label 'windows-agent'
    }

    triggers {
        pollSCM('H/2 * * * *')
    }

    stages {

        stage('Build') {
            steps {
                echo 'Building application...'
                bat 'echo Build completed'
            }
        }

        stage('Test') {
            steps {
                echo 'Testing application...'
                bat 'echo Test completed'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application...'
                bat 'echo Deployment completed'
            }
        }
    }
}
