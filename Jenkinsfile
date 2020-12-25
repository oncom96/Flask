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
        stage('Deploy') {
            steps {
                echo 'app.py'
            }
        }
        stage(‘Push Notification’) {
            steps {
                script{
                    withCredentials([string(credentialsId: ‘telegramToken’, variable: ‘1265469405:AAEYEBfgXQcY5iARmLmp6Hgw1wzHBHw0xkk’),
                        string(credentialsId: ‘telegramChatId’, variable: ‘492035825’)]) {
                            sh ”””

                                curl -s -X POST https://api.telegram.org/bot1265469405:AAEYEBfgXQcY5iARmLmp6Hgw1wzHBHw0xkk/sendMessage -d chat_id=492035825 -d parse_mode=”HTML” -d text=”<b>Project</b> : POC \
                                    <b>Branch</b>: master \
                                        <b>Build </b> : OK \
                                            <b>Test suite</b> = Passed”
            }
    }
            
