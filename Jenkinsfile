pipeline {
  agent {
    label 'jdk9'
  }
  stages {
    stage('Say Hello') {
      parallel {
        stage('Say Hello') {
          steps {
            echo 'Hello World!'
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
}