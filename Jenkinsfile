pipeline {
    agent any

    stages {
        stage ('Compile Stage') {
            steps {
                sh './gradlew clean build'
            }
        }

        stage ('Testing Stage') {

            steps {
                sh 'gradlew test'
            }
        }
    }
}