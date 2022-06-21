pipeline {
  agent {
    docker {
      image 'jenkins/jnlp-agent-docker:latest'
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