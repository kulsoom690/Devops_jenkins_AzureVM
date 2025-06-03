pipeline {
    agent any

    stages {
        stage('Pull Code') {
            steps {
                git 'https://github.com/YourUsername/jenkins-cicd-app.git'
            }
        }

        stage('Install Dependencies') {
            steps {
                sh 'npm install'
            }
        }

        stage('Run App') {
            steps {
                sh 'nohup node app.js &'
            }
        }
    }
}
