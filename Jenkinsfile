pipeline {
  agent {
    docker {
      image 'alexpilotti/ncsdk:1.11.00'
    }
    
  }
  stages {
    stage('Profile') {
      steps {
        sh '''cd tensorflow/inception_v3/
make profile'''
      }
    }
  }
}