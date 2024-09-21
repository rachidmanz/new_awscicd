pipeline {
    agent any

    environment {
        BRANCH_NAME = 'main'
        GIT_URL = 'https://github.com/rachidmanz/new_awscicd.git'
    }

    stages {
        stage('git checkout'){
            steps{
            git branch: "${BRANCH_NAME}", url: "${GIT_URL}"
            }
        }
        stage('docker build'){
            steps{
                sh 'docker build -t new_awscicd .'
                sh 'docker images'
            }
        }
        
    }
}
