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
    }
}