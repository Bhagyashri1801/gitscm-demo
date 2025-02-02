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
        withCredentials([string(credentialsID: 'mysecret', variable: 'mysecret')]){
          echo mysecret
        }
      }
    }
  }
}