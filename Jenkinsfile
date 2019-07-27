pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Running build automation'
        sh './gradle build --no-daemon'
        archiveArtefacts artefacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
