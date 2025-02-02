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
        withCredentials([string(credentialsId: 'mysecret', variable: 'mysecret')]) {
          // Use the GIT_CREDS variable here, for example to configure git authentication
          echo mysecret
       }
     }
    }
  }
}