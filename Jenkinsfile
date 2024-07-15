pipeline {
    agent any

    //environment {
      //  GITHUB_CREDENTIALS_ID = checkout([$class: 'GitSCM', branches: [[name: '*/main']], userRemoteConfigs: [[url: 'https://github.com/mohit435/test.git']]])
      //     }

   // stages {
     //   stage('Checkout') {
       //     steps {
                // Checkout the repository
         //       checkout([$class: 'GitSCM', branches: [[name: "*/${env.GIT_BRANCH}"]],
           //               userRemoteConfigs: [[url: env.GIT_REPO_URL, credentialsId: env.GITHUB_CREDENTIALS_ID]]])
     //       }
      //  }
    
    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                // Add your build steps here
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
                // Add your test steps here
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'
                // Add your deploy steps here
            }
        }
    }
}
