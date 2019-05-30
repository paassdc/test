pipeline {
  agent none
  stages {
    stage('step1') {
      parallel {
        stage('step1.1') {
          steps {
            echo 'hello!'
          }
        }
        stage('step1.2') {
          steps {
            echo 'hell!'
          }
        }
      }
    }
  }
  environment {
    Hell = 'O'
  }
}