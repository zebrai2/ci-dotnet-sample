pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'docker build .' 
                archiveArtifacts artifacts: '**/target/*.jar', fingerprint: true 
            }
        }
    }
}
