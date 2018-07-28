pipeline {
  agent any
  stages {
    stage ('build') {
      steps {
        echo 'Start running'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
