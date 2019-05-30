pipeline {
  agent none
  stages {
    stage('步骤1') {
      parallel {
        stage('步骤1.1') {
          steps {
            echo 'for a branch!'
          }
        }
        stage('步骤1.2') {
          steps {
            echo 'what the hell！'
          }
        }
      }
    }
    stage('step2') {
      steps {
        sleep 5
      }
    }
  }
  environment {
    Hell = 'O'
  }
}