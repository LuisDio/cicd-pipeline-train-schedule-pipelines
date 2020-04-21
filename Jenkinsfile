pipeline {
  agent any
  
  stages {
    stage('Build') {
      steps {
        echo 'Building application'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
