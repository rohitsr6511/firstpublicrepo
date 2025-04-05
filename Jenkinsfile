pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                script {
                    // Build the .NET console app
                    bat 'dotnet build'
                }
            }
        }
        stage('Publish') {
            steps {
                script {
                    // Publish the app to a folder
                    bat 'dotnet publish -c Release -o C:\Users\saini\Desktop\jenkisndeploy'
                }
            }
        }
        stage('Deploy') {
            steps {
                script {
                    // Run the .NET console app
                    bat 'C:\Users\saini\Desktop\jenkisndeploy\JenkinsDemo.exe'
                }
            }
        }
    }
}
