pipeline {
    agent none
    stages {
        stage('Check Agent') {
            agent any
            steps {
                echo 'Running on agent...'
                sh 'hostname'
                echo "Путь к воркспейсу: ${WORKSPACE}"
                echo "Имя текущей ноды: ${NODE_NAME}"
                }
            }

        stage('Build Info') {
            agent any
            steps {
                echo 'Build information...'
                echo 'Build number: ${BUILD_NUMBER}'
                echo 'Build ID: ${BUILD_ID}'
                echo 'Build URL: ${BUILD_URL}'
                }
            }

        stage('System Details') {
            agent any
            steps {
                sh 'uname -a'
                sh 'whoami'
                sh 'pwd'
                sh 'ls -la'
                sh 'free -h'
                sh 'date'
                }
            }
        }
}