pipeline {
    agent any
    tools {
        maven 'maven3'
    }
    stages {
        stage('Git Checkout') {
            steps {
                git branch: "prod", credentialsId: 'git-cred', url: 'https://github.com/bkrrajmali/cicd-jenkins.git'
            }
        }
        stage('Maven Compile') {
            steps {
                sh 'mvn compile'
            }
        }
    }
}