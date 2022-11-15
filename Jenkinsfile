pipeline {
  agent any
  stages {
    stage('stage1') {
      steps {
        sh '''pwd
date'''
      }
    }

    stage('stage2') {
      steps {
        sleep 10
      }
    }

    stage('stage 3') {
      steps {
        echo 'final step'
      }
    }

  }
}