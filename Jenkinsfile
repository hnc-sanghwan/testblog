node {
     stage('Clone repository') {
         checkout scm #repository를 jenkins workspace로 clone
     }

     stage('Build image') {
         app = docker.build("hnc-hskim/jenkins:$BUILD_NUMBER") #docker image build 및 이름을 hnc-hskim/jenkins:빌드번호 설정
     }
}
