pipeline {
  agent {
    docker {
      image 'image node:6.3'
    }

  }
  stages {
    stage('Build') {
      agent {
        docker {
          args '-p 3000:3000'
          image 'node:6.3'
        }

      }
      steps {
        sh 'npm install'
      }
    }
  }
}