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
          image 'node.6.3'
          args '-p 3000:3000'
        }

      }
      steps {
        sh 'npm install'
      }
    }
  }
}