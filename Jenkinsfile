pipeline {
    agent {
        node{
           label 'AGENT-1'
        }
    }
    stages {
        stage('Build') {
            steps {
                echo "Hi, I am Building"
            }
        }
        stage('Testing') {
            steps {
                echo "Hi I am testing"
            }
        }
        stage('Deploy') {
            steps {
                echo "Hi I am Deploying"
            }
        }
    }
}