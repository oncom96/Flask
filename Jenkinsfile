pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'app.py'
            }
        }
        stage('Test') {
            steps {
                sh 'app.py'
      
            }
        }
               stage('Deploy') {
                    steps {
                        sh 'app.py'
         }
     }
}

post {
        success {
            echo 'Build success'
            sh 'curl -d "chat_id=-292740675&text=Build success" https://api.telegram.org/bot1373771575:AAGWzfodFfnQH5pWuNMEzWoiUZ3JloBnhEI/sendMessage?chat_id=-292740675&text=Build'
        }
        
        failure {
            echo 'Build Automation'
            sh 'curl -d "chat_id=-292740675&text=Build Success" https://api.telegram.org/bot1373771575:AAGWzfodFfnQH5pWuNMEzWoiUZ3JloBnhEI/sendMessage?chat_id=-292740675&text=Success'
        }
    }
}
