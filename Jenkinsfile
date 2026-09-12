pipeline {
    agent {
        node{
           label 'AGENT-1'
        }
    }
    environment { 
        STATUS = "Success"
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
    post { 
        success { 
            echo 'I will run if "$STATUS"'
            echo " $STATUS "
        }
        failure { 
            echo 'I will run if failure'
        }
        always {
            echo 'I will say hello again'
            cleanWs()
        }
    }
}