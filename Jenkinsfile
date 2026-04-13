pipeline {
    agent any
    stages {
        stage('Variables Demo') {
            script {
                def appName = "MyApplication"
                def port =  8080
                def isProduction = false
            }
            steps {
                echo "${appName}"
                echo "${port}"
                echo "${isProduction}"
            }
        }

        stage('String Operations') {
            script {
                def message = "Jenkins Pipeline Tutorial"
                def new_message = "${message.replace('Tutorial', 'Course')}"
            }
            steps {
                echo "Length: ${message.length()}"
                echo "toUpperCase: ${message.toUpperCase()}"
                echo "toLowerCase: ${message.toLowerCase()}"
                echo "New Message: ${new_message}"
            }

        }}
    }
}