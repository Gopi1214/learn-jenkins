pipeline {
    agent { 
        node { 
            label 'AGENT-1' 
            } 
        }
    environment { 
        GREETING = 'I will not stop anymore'
    }
    // Build
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
        
                // sleep 35
                sh """
                   echo "hello AMMA I love you so much amma I am ready to sacrifice my life for you"
                   echo $GREETING
                """
            }
        }
    }
    // Post Build
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