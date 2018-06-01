pipeline {
  agent any
  stages {
    stage('stage1') {
      parallel {
        stage('stage1') {
          steps {
            echo 'hahaha'
          }
        }
        stage('stage2') {
          steps {
            echo 'bishyoumadeittothenextstep'
            timeout(time: 2, activity: true) {
              echo 'bishwait'
            }

          }
        }
      }
    }
    stage('superstage') {
      steps {
        echo 'woah!!!!youmadeittosuperstage!!!:o'
        sleep 4
      }
    }
  }
}