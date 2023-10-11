pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        docker { image 'node:16-alpine' }
        sh 'npm install --version'
      }
    }
  }
}
