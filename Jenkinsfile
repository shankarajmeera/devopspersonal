pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'build success '
      }
    }

    stage('test') {
      environment {
        CI = 'true'
      }
      steps {
        sh './jenkins/scripts/test.sh'
      }
    }

  }
}