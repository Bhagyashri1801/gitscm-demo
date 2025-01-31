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
        withcredentials([string(credentialsID: 'mysecret', variable: 'mysecret')]){
        echo mysecret
        }
      }
    }
  }
}
