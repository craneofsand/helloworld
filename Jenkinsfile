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
        sh 'echo "Test Stage"'
        sh 'sh ./scripts/test.sh'
      }
    }

  }
}
