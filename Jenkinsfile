pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            retry(count: 1) {
              echo 'Jenkins Build'
            }

          }
        }
        stage('run code') {
          steps {
            sh 'echo "Hello"'
          }
        }
        stage('rerun') {
          steps {
            sleep 4
          }
        }
      }
    }
    stage('Success message') {
      steps {
        echo 'Success'
      }
    }
  }
}