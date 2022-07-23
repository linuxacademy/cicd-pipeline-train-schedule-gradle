pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Running build automation-branch-1'
                sh './gradlew build --no-daemon'
                archiveArtifacts artifacts: 'dist/trainSchedule.zip'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing Stage-branch-1'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploy Stage-branch-1'
            }
        }

    }
}
