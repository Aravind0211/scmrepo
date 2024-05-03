pipeline {
    agent any
    stages {
        stage('Build'){
            tools{
                jdk 'java-1.8'
            }
            steps{
                sh'./gradlew build'
            }
        }
    }
}
