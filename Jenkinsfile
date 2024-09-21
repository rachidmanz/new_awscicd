pipeline {
    agent any

    stages {
        stage('git checkout'){
            steps{
            git branch: 'main', url: 'https://github.com/rachidmanz/new_awscicd.git'
            }
        }
        stage('test'){
            steps{
                sh 'echo test'
            }
        }
        stage('test2'){
            steps{
                sh 'echo test2'
            }
        }
    }
}
