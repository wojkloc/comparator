pipeline {
    agent any

    stages {
        stage ('Compile Stage') {
            steps {
                sh 'sudo chmod +x gradlew'
                sh 'sudo ./gradlew clean build --info'
            }
        }

        stage ('Testing Stage') {

            steps {
                sh 'sudo ./gradlew test -s'
            }
        }
    }
}