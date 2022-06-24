pipeline {
  agent any {
    stages {
      stage {
        steps ('Build') {
          echo "Running Build Automation"
          sh './gradlew build --no-daemon'
          archiveArtifacts artifacts: 'dist/trainSchedule.zip'
        }
      }
    }
  }
}
