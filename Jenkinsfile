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
          }
        }
      }
    }
  }
}