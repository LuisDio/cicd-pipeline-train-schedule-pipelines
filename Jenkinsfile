pipeline {
  agent any
  
  stages {
    stage('Build') {
      step {
        echo 'Building application'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
