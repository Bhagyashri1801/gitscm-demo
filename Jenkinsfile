pipeline {
  agent any

  stages {
    stage('Hello') {
      steps {
        echo 'Hello World'
      }
    } 
    stage('Build') {
      steps {
        withCredentials([string(credentialsID: 'mysecret',variable: 'mysecret')]){
        echo 'mysecret'
         }
      }
    }
  }
}
