pipeline {
    agent any
    stages {
        stage('Build'){
            tools {
                jdk 'java-8'
           }
            steps{
                sh'./gradlew build'
            }
        }
    }
}
