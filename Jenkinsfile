// Jenkinsfile
// Мой первый пайплайн

pipeline {
    agent any
    stages {
        stage('Hello') {
            steps {
                echo 'Привет от Jenkins и Просто Девопс!'
                echo 'Сегодняшняя дата:'
                sh 'date'
            }
        }

        stage('System Info') {
            steps {
                echo 'Информация о системе:'
                echo 'Операционная система:'
                sh 'uname -a'
                echo 'Текущая директория:'
                sh 'pwd'
                echo 'Список файлов:'
                sh 'ls -la'
            }
        }

        stage('Install deps') {
            steps {
                sh '''
                    python3 -m venv venv
                    . venv/bin/activate
                    pip install --upgrade pip
                    pip install pytest
                '''
            }
        }

        stage('Tests') {
            steps {
                sh 'pytest'
            }
        }
    }
}