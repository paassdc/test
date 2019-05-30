pipeline {
  agent none
  stages {
    stage('step1') {
      parallel {
        stage('step1.1') {
          steps {
            echo 'for a branch!'
          }
        }
        stage('step1.2') {
          steps {
            echo 'what the hell!'
          }
        }
      }
    }
    stage('step2') {
      steps {
        sleep 5
      }
    }
    stage('step3') {
      parallel {
        stage('step3.1') {
          steps {
            echo 'build a repo here!'
          }
        }
        stage('step3.2') {
          agent any
          steps {
            echo 'send email'
            timestamps() {
              echo 'timestamp child?'
            }

          }
        }
      }
    }
    stage('step4') {
      steps {
        echo '44444'
      }
    }
    stage('step5') {
      steps {
        sleep(unit: 'SECONDS', time: 10)
        timestamps() {
          sleep 4
          echo 'what\'s the time?'
        }

      }
    }
  }
  environment {
    Hell = 'O'
  }
}
