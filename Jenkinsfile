pipeline {
    agent any

    stages {
        stage ('Compile Stage') {
            sh './gradlew clean build'
        }

        stage ('Testing Stage') {
            sh './gradlew test'
        }
    }
}