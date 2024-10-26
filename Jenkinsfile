pipeline {
    agent any
    stages {
        stage('Git Checkout') {
            steps {
                git branch: "prod", url: 'https://github.com/bkrrajmali/cicd-jenkins.git'
            }
        }
    }
}