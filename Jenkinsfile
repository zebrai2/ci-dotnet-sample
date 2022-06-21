pipeline {
  agent {
    docker {
      image 'jenkins/jnlp-agent-docker'
    }

  }
  stages {
    stage('Verification') {
      steps {
        withDockerServer([uri: 'dind']) {
            sh 'docker build /ci-dotnet-sample/Dockerfile .'
        }
      }
    }

  }
}
