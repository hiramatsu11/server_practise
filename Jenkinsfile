pipeline {
    agent any

    stages {
        stage('Clonar repo'){
            steps {
                git branch: 'main', url: 'https://github.com/hiramatsu11/server_practise.git'
            }
        }
        stage('Ejecutar hello.py'){
            steps {
                sh 'python3 hello.py'
            }
        }
    }
}