pipeline {
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
            }
        }

        stage('Run Java') {
            steps {
                sh 'java demo'
            }
        }

        stage('Run Python') {
            steps {
                sh 'python3 hello.py'
            }
        }
    }
}
