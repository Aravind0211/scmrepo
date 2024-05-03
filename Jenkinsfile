pipeline {
    agent any
    stages {
        stage('Build'){
            tools {
                jdk 'java-8'
           }
            steps{
                sh'chmod -R 777.'
                sh'./gradlew build'
            }
        }
    }
}
