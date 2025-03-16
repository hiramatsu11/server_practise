pipeline {
    agent any

    stages {
        stage('Clonar repo'){
            steps {
                git branch: 'main', url: 'https://github.com/hiramatsu11/server_practise.git'
            }
        }
        stage('Donde esta python3'){
            steps {
                sh 'which python3'
            }
        }
        stage('Ejecutar hello.py'){
            steps {
                sh '/usr/bin/python3 hello.py'
            }
        }
    }
}