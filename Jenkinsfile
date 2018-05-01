pipeline {
  agent {
    label 'jdk8'
  }
  stages {
    stage('Say Hello') {
      parallel {
        stage('Say Hello') {
          steps {
            echo 'Hello ${MY_NAME}!'
            sh 'java -version'
          }
        }
        stage('say hello') {
          steps {
            echo 'Hello World!'
            sh 'java -version'
          }
        }
      }
    }
  }
  environment {
    MY_NAME = 'Mary'
  }
}