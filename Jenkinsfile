pipeline {
    agent any
    environment {
        GIT_URL = 'https://github.com/Bhagyashri1801/gitscm-demo.git'
    }
    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }
        stage('Hello') {
            steps {
                echo 'Hello Bhagu'
            }
        }
        stage('Build') {
            steps {
                withCredentials([string(credentialsId: 'mysecret', variable: 'mysecret')]) {
                    // Use the GIT_CREDS variable here, for example to configure git authentication
                    echo "mysecret"
                }
            }
        }
    }
}
