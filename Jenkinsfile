pipeline {
  agent any
  stages {
    stage('first') {
      parallel {
        stage('first') {
          agent any
          steps {
            sh '''
echo `hostname`'''
          }
        }

        stage('docker show images') {
          steps {
            sh '''
sudo docker images'''
          }
        }

      }
    }

  }
}