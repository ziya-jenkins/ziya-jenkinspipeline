pipeline {
  agent any
  stages {
    stage('Say Hello') {
      parallel {
        stage('Say Hello') {
          steps {
            echo 'Hello World!'
            sh '''pipeline {
   agent any
   stages {
      stage(\'Say Hello\') {
         steps {
            echo \'Hello World!\'   
            sh \'java -version\'
         }
      }
   }
}'''
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