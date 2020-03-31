pipeline {
    agent any

    stages {
        stage('Create') {
            steps {
                sh './gradlew build --no-daemon'
            }
        }
    }
}