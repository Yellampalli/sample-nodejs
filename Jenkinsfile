pipeline {
    agent any 
    stages { 
        stage('SCM Checkout') {
            steps{
            git 'https://github.com/kaza514/sample-nodejs.git'
            }
        }

        stage('Build docker image') {
            steps {  
                sh 'docker build -t kaza514/nodeapp:$BUILD_NUMBER .'
            }
        }
    }
}

