pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                bat 'gradle build -x test'
            }
        }

    }

    post {
        success {
            echo 'Gradle build successful!'
        }

        failure {
            echo 'Gradle build failed!'
        }
    }
}