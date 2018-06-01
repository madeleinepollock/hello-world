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
            error 'whoops'
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