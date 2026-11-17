opipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Compile Java') {
            steps {
                sh 'javac demo.java'
                echo 'build started'
            }   
        }

        stage('Run Java') {
            steps {
                sh 'java demo'
                echo 'build'
            }
        }

        stage('Run Python') {
            steps {
                sh 'python3 hello.py'
            }
        }
    }
}
