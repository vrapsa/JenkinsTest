pipeline {
    agent any
    stages {
        stage('Check Agent') {
            steps {
                echo 'Running on agent...'
                sh 'hostname'
                sh 'go build -o app /var/jenkins_home/workspace/check-agent/'
                echo "Путь к воркспейсу: ${WORKSPACE}"
                echo "Имя текущей ноды: ${NODE_NAME}"
}
}
}
}