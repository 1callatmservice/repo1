pipeline{
    agent any
    environment{
        staging_server="172.104.62.106"
    }
    stages{
        stage('Deploy to Remote'){
            steps{
                
                 sh 'scp -o StrictHostKeyChecking=no -r ${WORKSPACE}/pull/* thinksurfmedia@${staging_server}:/home6/thinksurfmedia/public_html/'
                 
            }
        }
    }
}
