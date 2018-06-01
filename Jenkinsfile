pipeline {
  agent any
  stages {
    stage('stage1') {
      parallel {
        stage('stage1') {
          steps {
            echo 'hahaha'
            build(job: 'yoyoyo', propagate: true, quietPeriod: 1)
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