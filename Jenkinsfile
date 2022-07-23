pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Running build automation'
                sh './gradlew build --no-daemon'
                archiveArtifacts artifacts: 'dist/trainSchedule.zip'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing Stage'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploy Stage'
            }
        }

    }
}
