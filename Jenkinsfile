pipeline {
  agent any
  stages {
    stage('Hello') {
      steps {
        echo 'Hello Bhagu'
      }
    } 
    stage('Build') {
      steps {
        withCredentials([string(credentialsId: 'git-credential', variable: 'GIT_CREDS')]) {
          // Use the GIT_CREDS variable here, for example to configure git authentication
          echo "Using credentials"
       }
     }
    }
  }
}