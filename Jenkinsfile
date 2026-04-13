pipeline {
    agent any
    stages {
        stage('Variables Demo') {
            steps {


            script {
                def appName = "MyApplication"
                def port =  8080
                def isProduction = false
                echo "${appName}"
                echo "${port}"
                echo "${isProduction}"
                }
            }
        }

        stage('String Operations') {
        steps {
            script {
                def message = "Jenkins Pipeline Tutorial"
                def new_message = "${message.replace('Tutorial', 'Course')}"
                echo "Length: ${message.length()}"
                echo "toUpperCase: ${message.toUpperCase()}"
                echo "toLowerCase: ${message.toLowerCase()}"
                echo "New Message: ${new_message}"
                }
            }
        }

        stage('Build Version') {
            steps {
                script {
                def major = '1'
                def minor = '0'
                def env.APP_VERSION = "${major}.${minor}.${env.BUILD_NUMBER}}"
                echo "Application version: ${env.APP_VERSION} "
                }
            }
        }
    }
}