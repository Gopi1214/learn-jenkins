pipeline {
    // agent none
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
            }
        }
    }
}