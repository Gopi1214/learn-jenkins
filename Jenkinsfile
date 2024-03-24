pipeline {
    agent { 
        node { 
            label 'AGENT-1' 
            } 
        }
    stages {
        stage('Build') { 
            steps {
                echo "hello"
            }
        }
        stage('Test') { 
            steps {
                echo "hi"
            }
        }
        stage('Deploy') { 
            steps {
                echo "good morning"
                sleep 35
            }
        }
    }
    post { 
        always { 
            echo 'I will always say Hello again!'
        }
        failure { 
            echo 'I will run when the job has failed!'
        }
        success { 
            echo 'I will run when the job is success!'
        }
        aborted { 
            echo 'I will run when the job is aborted manually!'
        }
    }
}