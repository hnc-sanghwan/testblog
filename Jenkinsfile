def templatePath = 'https://raw.githubusercontent.com/openshift/nodejs-ex/master/openshift/templates/nodejs-mongodb.json' 
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
      }
    } 
  }
}
