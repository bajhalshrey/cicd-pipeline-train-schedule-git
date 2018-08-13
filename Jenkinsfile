pipeline {
  agent any
  stages {
    stage ('Build') { 
      steps {
        echo 'Running build automation'
        sh './gradlew build --no-daenmon'
        archiveArtifcats artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
