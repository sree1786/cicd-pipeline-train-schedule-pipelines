pipeline{
  agent any
  stages{
    stage ('Build') {
      steps {
        echo 'running build automaction'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
        
      }
    }
  }
}
