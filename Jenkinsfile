pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                checkout scmGit(branches: [[name: '*/master']], extensions: [], userRemoteConfigs: [[credentialsId: 'github', url: 'https://github.com/web3j/sample-project-gradle.git']])
            }
        }
        stage('Build') {
            steps {
                sh './gradlew build'
            }
        }
    }
}
