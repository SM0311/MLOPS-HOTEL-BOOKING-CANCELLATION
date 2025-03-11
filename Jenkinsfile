pipeline{
    agent any

    environment {
        VENV_DIR = 'venv'
    }

    stages{
        stage('Cloning Github repo to Jenkins'){
            steps{
                script{
                    echo 'Cloning Github repo to Jenkins..........'
                    checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'github-token', url: 'https://github.com/SM0311/MLOPS-HOTEL-BOOKING-CANCELLATION.git']])
                }
            }
        }

        stage('Setting up our Virtual Enviornment and Installing dependencies'){
            steps{
                script{
                    echo 'Setting up our Virtual Enviornment and Installing dependencies..........'
                    sh '''
                    python -m venv ${VENV_DIR}
                    . ${VENV_DIR}/bin/activate
                    pip install --upgrade pip
                    pip install -e .
                    '''
                }
            }
        }
    }
}