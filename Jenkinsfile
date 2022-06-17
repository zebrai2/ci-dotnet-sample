pipeline {
  agent {
    dockerfile {
      filename 'ci-dotnet-sample/Dockerfile'
    }

  }
  stages {
    stage('error') {
      steps {
        sh 'docker build . -t test'
      }
    }

  }
}