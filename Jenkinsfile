def credential = 'ade-test'
def server = 'ads@103.176.79.216'
def dir ='/home/ads/literature-frontend'
def branch = 'main'

pipeline{
    agent any
    stages{
        stage('Pull test'){
            steps{
                sshagent([credential]){
                    sh """ssh -o StrictHostKeyChecking=no ${server} << EOF
                    echo "Pulling Wayshub Backend Repository"
                    cd ${dir}
                    git pull origin ${branch}
                    exit
                    EOF"""
                    }
                }
            }
        }
    }
