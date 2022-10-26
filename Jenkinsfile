pipeline{
  agent any
  // tools {
  //   nodejs 'node-14.20.1'
  // }
  options {
    timeout(time: 2, unit: 'MINUTES')
  }
  stages {
    stage('Install dependencies') {
      steps {
        sh 'cd test-jenkins && npm install'
      }
    }
    stage('Run tests') {
      steps {
        sh 'cd test-jenkins && npm run test'
      }
    }
  }
}