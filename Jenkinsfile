pipeline {
    agent any

    stages {
        stage('Create') {
            steps {
                sh './gradlew build --no-daemon'
            }
        }
    }
    post {
        always {
            archiveArtifacts artifacts: 'dist/trainSchedule.zip', fingerprint: true
        }
    }
}