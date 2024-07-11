pipeline {
    agent any

    stages {
        stage('Clone Repository') {
            steps {
                git url: 'git@github.com:your-username/your-private-repo.git', credentialsId: 'your-credentials-id'
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
        stage('Deploy') {
            steps {
                // Add your deploy steps here
                echo 'Deploying...'
            }
        }
    }
}
