pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        retry(count: 1) {
          echo 'Jenkins Build'
        }

      }
    }
  }
}