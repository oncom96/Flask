pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'app.py'
            }
        }
        stage('Test') {
            steps {
                echo 'app.py'
            }
        }
        stage('TelegramBot') {
            steps {
                script{
                    withCredentials([string(credentialsId: ‘telegramToken’, variable: ‘1265469405:AAEYEBfgXQcY5iARmLmp6Hgw1wzHBHw0xkk’),
                        string(credentialsId: ‘telegramChatId’, variable: ‘492035825’)]) {
            }
        }
                stage('Deploy') {
                    steps {
                        echo 'app.py'   
            }
    }
         
        
