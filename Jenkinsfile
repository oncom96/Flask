pipeline {
    agent { docker { image 'Python:3.8.5' } }

    stages {
        stage('Build') {
            steps {
                sh 'python3 -V'
            }
        }
        stage('Test') {
            steps {
                echo 'app.py'
                sh 'curl -d app.py'
      
            }
        }
               stage('Deploy') {
                    steps {
                        sh 'python3 -V'
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
