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
             post {
                success {
                    echo 'Build success'
                        sh 'curl -d https://api.telegram.org/bot1265469405:AAEYEBfgXQcY5iARmLmp6Hgw1wzHBHw0xkk/sendMessage?chat_id=492035825&text=Build success'
        }
        
        failure {
            echo 'Build failure'
            sh 'curl -d https://api.telegram.org/bot1265469405:AAEYEBfgXQcY5iARmLmp6Hgw1wzHBHw0xkk/sendMessage?chat_id=492035825&text=Build failure'
        }
    }
}
