pipeline {

  agent any
  stages {
  
    stage('Build project') {
      steps {
      
        echo 'Building the project'
        
        sh './gradlew build --no-daemon'
        
        archiveArticfacts artifacts: 'dist/trainSchedule.zip'
      
      }
    }
  }
}
