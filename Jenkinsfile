pipeline {
    agent any

    stages {
        stage ('Compile Stage') {
            steps {
                sh 'sudo chmod +x gradlew'
                sh 'sudo ./gradlew clean build -s'
            }
        }

        stage ('Testing Stage') {

            steps {
                sh 'sudo ./gradlew test -s'
            }
        }
    }
}