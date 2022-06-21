pipeline {
  agent {
    docker {
      image 'jenkins/jnlp-agent-docker:latest'
    }

  }
  stages {
    stage('error') {
      steps {
        sh 'docker --version'
      }
    }

  }
}