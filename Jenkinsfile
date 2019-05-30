#!groovy
pipeline {
  agent none
  stages {
    stage('步骤1') {
      parallel {
        stage('步骤1.1') {
          steps {
            echo 'hello！'
          }
        }
        stage('步骤1.2') {
          steps {
            echo 'hell！'
          }
        }
      }
    }
  }
  environment {
    Hell = 'O'
  }
}
