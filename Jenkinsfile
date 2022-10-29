pipeline {
  agent {
    docker { image 'node:16-alpine' }
  }
  stages {
    stage('Test') {
      steps {
        sh 'npm version'
      }
    }
    stage('Build') {
      steps {
        sh 'npm start'
      }
    }
  }
}
