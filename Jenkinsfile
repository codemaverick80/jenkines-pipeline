pipeline {
    agent any
    stages {
        stage('Restore packages'){
           steps{
               sh 'dotnet restore'
            }
         }
        stage('Clean'){
           steps{
               sh 'dotnet clean --configuration Release'
            }
         }
        stage('Build'){
           steps{
               sh 'dotnet build --configuration Release --no-restore'
            }
         }
     }
}