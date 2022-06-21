pipeline {
  agent {
    docker {
      image 'jenkins/jnlp-agent-docker'
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