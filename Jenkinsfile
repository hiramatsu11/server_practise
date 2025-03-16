pipeline {
    agent any

    stages {
        stage('Clonar repo'){
            steps {
                git branch: 'main', url: 'https://github.com/hiramatsu11/server_practise.git'
            }
        }
        stage('Instalar python si es necesario') {
            steps {
                sh '''
                if ! command -v python3 & /dev/null
                then
                    echo "Python3 no encontrado, instalando"
                    sudo apt update && sudo apt install -y python3
                else
                    echo "Pytho3 ya esta instalado"
                fi
                '''
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