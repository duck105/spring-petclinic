pipeline {
  agent any
  stages {
    stage('SonarQube') {
      steps {
        withSonarQubeEnv('sonar_server') {
          sh '''./mvnw org.sonarsource.scanner.maven:sonar-maven-plugin:4.7.0.2747:sonar
'''
        }

      }
    }

  }
}