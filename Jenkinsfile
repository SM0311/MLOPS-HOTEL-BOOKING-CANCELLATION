pipeline{
    agent any

    stages{
        stage('Cloning Github repo to Jenkins'){
            steps{
                script{
                    echo 'Cloning Github repo to Jenkins..........'
                    checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'github-token', url: 'https://github.com/SM0311/MLOPS-HOTEL-BOOKING-CANCELLATION.git']])
                }
            }
        }
    }
}