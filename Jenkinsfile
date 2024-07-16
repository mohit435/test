// pipeline {
//     agent any

//     environment {
//         GITHUB_CREDENTIALS_ID = checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'GitHub', 
//                                                                                                                    url: 'https://github.com/mohit435/test.git']])
//            }

//     stages {
//        stage('Checkout') {
//             steps {
//                 // Checkout the repository
//                 checkout([$class: 'GitSCM', branches: [[name: "*/${env.GIT_BRANCH}"]],
//                           userRemoteConfigs: [[url: env.GIT_REPO_URL, credentialsId: env.GITHUB_CREDENTIALS_ID]]])
//             }
//         }
    
//    stages {
//         stage('Build') {
//             steps {
//                 echo 'Building...'
//                 // Add your build steps here
//             }
//         }
//         stage('Test') {
//             steps {
//                 echo 'Testing...'
//                 // Add your test steps here
//             }
//         }
//         stage('Deploy') {
//             steps {
//                 echo 'Deploying...'
//                 // Add your deploy steps here
//             }
//         }
//     }
// }


pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/mohit435/test.git'
            }
        }
        stage('Run Test') {
            steps {
                sh 'chmod +x test'  // Ensure script is executable if needed
                sh './test'         // Execute the test script
            }
        }
    }
}

