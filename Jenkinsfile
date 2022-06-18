pipeline {
  agent {
    dockerfile {
      filename 'ci-dotnet-sample/Dockerfile'
    }

  }
  stage('Build'){ 
          docker.build(imageName) 
  }
}
