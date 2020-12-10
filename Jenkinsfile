pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo 'Running build automation'
        sh './gradlew build --no-daemon'
        echo 'archiving'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
