pipeline {
  agent {
    dockerfile true
  }
  stages {
    stage('error') {
      steps {
        sh 'docker --version'
      }
    }

  }
}