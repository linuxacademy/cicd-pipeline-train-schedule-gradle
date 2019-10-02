pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo 'Running build automation'
        sh './gradlew build --no-daemon --console plain'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
