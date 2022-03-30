pipeline {
  agent any
  stages {
    stage('Analyze') {
      steps {
        withSonarQubeEnv(installationName: 'sonar_server', credentialsId: 'ef5782996c1b5f9b6dbac3b1e7021c3f989b2556') {
          sh './mvnw clean verify sonar:sonar'
        }

      }
    }

  }
}