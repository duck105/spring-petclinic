pipeline {
  agent any
  stages {
    stage('Analyze') {
      steps {
        sh './mvnw clean verify sonar:sonar -Dsonar.login=ef5782996c1b5f9b6dbac3b1e7021c3f989b2556'
      }
    }

    stage('Build') {
      steps {
        sh './mvnw package'
      }
    }

  }
}