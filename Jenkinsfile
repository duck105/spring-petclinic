pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh './mvnw spring-boot:run'
      }
    }

    stage('SonarQube') {
      steps {
        withSonarQubeEnv 'sonar_server'
      }
    }

  }
}