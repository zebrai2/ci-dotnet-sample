pipeline {
  agent {
    dockerfile {
      filename './ci-dotnet-sample/Dockerfile'
    }

  }
  stages {
    stage('Build') {
      steps {
        sh 'docker build .'
      }
    }

  }
}