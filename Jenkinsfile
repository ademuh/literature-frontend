def credential = 'ade-test'
def server = 'ads@103.176.79.216'
def dir ='/home/ads/literature-frontend'
def branch = 'main'

pipeline{
    agent any
    stages{
        stage('yeet'){
            steps{
                sshagent([credential]){
                    sh """ssh -o StrictHostKeyChecking=no ${server} << EOF
                    echo "yeet"
                    exit
                    EOF"""
                    }
                }
            }
        }
    }
