pipeline {
    agent none
    options { skipDefaultCheckout(true) }
    stages {
        stage('Build') {
            agent {
                docker {
                    image 'node:11-alpine'
                }
            }
            options { skipDefaultCheckout(false) }
            steps {
                sh 'npm install'
                sh 'npm run build'
            }
        } 
    }
}
