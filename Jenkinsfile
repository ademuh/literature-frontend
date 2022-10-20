def credential = 'ade-test'
def server = 'ads@103.176.79.216'
def dir ='/home/ads/literature-frontend'
<<<<<<< HEAD
def branch = 'main'
=======
def branch = 'development'
>>>>>>> 8ac23565ac01eb9f9c99227b98dd03345707f65f

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
