pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/raulcoast/meuappflutter'
            }
        }

        stage('Build') {
            steps {
                sh 'flutter build apk' // Comando para construir um app Flutter
            }
        }

        stage('Test') {
            steps {
                sh 'flutter test' // Executa testes do Flutter
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application...'
                // Aqui você pode adicionar comandos para publicação
            }
        }
    }
}