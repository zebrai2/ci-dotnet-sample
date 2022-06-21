pipeline {
  agent {
    docker {
      image 'dind:latest'
    }

  }
  stages {
    stage('Verification') {
      steps {
        sh 'docker --version'
      }
    }

  }
}