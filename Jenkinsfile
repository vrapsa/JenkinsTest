pipeline {
    agent {
        docker {
            image 'python:3.11'
        }
    }

    stages {
        stage('Hello') {
            steps {
                echo 'Привет от Jenkins!'
                sh 'date'
            }
        }

        stage('System Info') {
            steps {
                sh 'uname -a'
                sh 'pwd'
                sh 'ls -la'
            }
        }
    }
}