pipeline {
    agent any
    stages {
        stage('Build') {
           steps {
               echo 'Started Build Automation'
               sh './gradlew build --no-daemon'
               echo 'Completed Build Automation'
               archiveArtifacts artifacts: 'dist/trainSchedule.zip'
	       echo 'Test'
           }
        }
    }
}
