node {
     stage('Clone repository') {
         checkout scm
     }

     stage('Build image') {
         app = docker.build("hnc-hskim/jenkins:$BUILD_NUMBER")
     }
}
