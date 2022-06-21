pipeline{
    agent none
    stages{
        stage('stage_name'){
            steps {
                agent {
                    dockerfile{
                    dir 'ci-dotnet-sample/Dockerfile'
                    }
                }
            }
         }
    }
}


