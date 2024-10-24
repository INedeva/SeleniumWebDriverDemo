pipeline {
    agent any
    stages {
        stage('Restore Dependencies') {
            steps {
                bat 'dotnet restore'
            } 
        }
        stage('Build') {
            steps {
                bat 'dotnet build'
            } 
        }
        stage('Test1') {
            steps {
                bat 'dotnet test TestProject1/TestProject1.csproj'
            } 
        }
        stage('Test2') {
            steps {
                bat 'dotnet test TestProject2/TestProject2.csproj'
            } 
        }
        stage('Test3') {
            steps {
                bat 'dotnet test TestProject3/TestProject3.csproj'
            } 
        }
    }
}