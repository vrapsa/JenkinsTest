pipeline {
    agent any

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