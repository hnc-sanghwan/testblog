def templateName = 'testblog' 
pipeline {
  agent {
    node {
      label 'nodejs' 
    }
  }
  options {
    timeout(time: 20, unit: 'MINUTES') 
  }
  stages {
    stage('Build') {
      steps {
          sh 'npm install'
          sh 'npm run build'
      }
    } 
  }
}
