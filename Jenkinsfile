pipeline {
  agent any
  stages {
    stage {'Build'} {
      steps {
        echo 'Running buiuld automation'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
