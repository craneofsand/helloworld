pipeline {
  agent any
  stages {
    stage('Build') {
      environment {
        CI = 'true'
      }
      steps {
        sh 'echo "Build Stage"'
        sh 'sh ./scripts/build.sh'
      }
    }

    stage('Test') {
      steps {
        sh 'echo "########"'
        sh 'sh ./scripts/test.sh'
      }
    }

  }
}