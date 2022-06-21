pipeline{
    agent none
    stages{
        stage('stage_name'){
            agent {
                dockerfile{
                label 'my-build'
                dir ' ci-dotnet-sample/Dockerfile'
                }
            }
         }
    }
}


