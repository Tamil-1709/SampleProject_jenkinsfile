pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/Tamil-1709/Test_DevOps_SampleProject'
            }
        }
        stage('Build') {
            steps {
                bat 'dotnet build'
            }
        }
        stage('Test') {
            steps {
                bat 'dotnet test'
            }
        }
        stage('Deploy') {
            steps {
                bat 'dotnet publish -c Release'
            }
        }
    }
}
 
