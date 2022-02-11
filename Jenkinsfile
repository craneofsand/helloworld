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

  }
}