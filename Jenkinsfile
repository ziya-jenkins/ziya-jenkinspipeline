pipeline {
  agent {
    label 'jdk8'
  }
  stages {
    stage('Say Hello') {
      parallel {
        stage('Say Hello') {
          steps {
            echo "Hello ${MY_NAME}!"
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
    TEST_USER = credentials('test-user')
  }
  parameters {
    string(name: 'Name', defaultValue: 'whoever you are', description: 'Who should I say hi to?')
  }
}