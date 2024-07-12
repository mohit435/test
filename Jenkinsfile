pipeline {
    agent any

    stages {
        stage('Clone Repository') {
            steps {
                checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'GitHub', url: 'https://github.com/mohit435/test.git']])
            }
        }
        stage('Build') {
            steps {
                // Add your build steps here
                echo 'Building...'
            }
        }
        stage('Test') {
            steps {
                // Add your test steps here
                echo 'Testing...'
            }
        }
         stage('SonarQube Analysis') {
            steps {
                withSonarQubeEnv('SonarQube') {
                    sh 'sonar-scanner'
                }
            }
        }
        stage('Deploy') {
            steps {
                // Add your deploy steps here
                echo 'Deploying...'
            }
        }
    }
}
