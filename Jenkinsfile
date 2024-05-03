pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'github', url: 'https://github.com/Aravind0211/scmrepo.git']])
            }
        }
        stage('Build'){
            steps{
                //sh 'chmod -R 777 .'
                sh './gradlew build'
            }
        }
        stage('Unit Test'){
            tools{
                jdk 'java-8'
            }
            steps{
                sh './gradlew test'
            }
        }
    }
}
