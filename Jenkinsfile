pipeline {
  agent any
  stages {
    stage('Hello') {
      steps {
        sh '''
                date
                pwd
                ls
                '''
      }
    }

    stage('Hello2') {
      steps {
        sh 'echo "${BUILD_NUMBER}"'
        sh 'echo "${name}"'
        sh 'echo "${uname}"'
        sh 'echo "${person}"'
      }
    }

    stage('Hello3') {
      environment {
        uname = 'admin00'
      }
      steps {
        echo 'Hello World3'
        sh 'echo "${name}"'
        sh 'echo "${uname}"'
      }
    }

  }
  environment {
    name = 'adminp'
  }
  parameters {
    string(name: 'person', defaultValue: 'Enter Name', description: 'Enter full name')
  }
}