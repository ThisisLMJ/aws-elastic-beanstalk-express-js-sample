pipeline {
  agent any
  stages {
    stage('clone'){
      steps{
        git url: 'https://github.com/ThisisLMJ/aws-elastic-beanstalk-express-js-sample', branch: 'main'
      }
    stage('Build') {
      steps {
        docker { image 'node:16-alpine' }
        sh 'npm install --version'
      }
    }
  }
}
