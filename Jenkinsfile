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
                        sh 'curl -d "chat_id=-492035825&text=Build success" https://api.telegram.org/bot<token>/sendMessage'
        }
        
        failure {
            echo 'Build failure'
            sh 'curl -d "chat_id=-492035825&text=Build failure" https://api.telegram.org/bot<token>/sendMessage'
        }
    }
}
        
