pipeline {
    agent any

    stages {
        stage ('Compile Stage') {

            steps {
                withGradle(gradle : 'gradle 4.10.3') {
                    sh 'gradlew build'
                }
            }
        }

        stage ('Testing Stage') {

            steps {
                withGradle(gradle : 'gradle 4.10.3') {
                    sh 'gradlew test'
                }
            }
        }
    }
}