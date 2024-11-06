pipeline {
    agent any
    stages {
        stage('Build'){
            steps{
                bat 'npm install'
                powershell '''
                 write-Output "Hello World!"
                 $date = Get-Date
                 write-Output "Current Date and time is : $date" 
                '''
                powershell '''C:\\My-Script\\MyScript.ps1'''
            }
        }
    }
}