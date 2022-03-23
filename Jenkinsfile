pipeline {
  agent any
  stages {
    stage('SonarQube') {
      steps {
        withSonarQubeEnv('sonar_server') {
          sh 'sh \'mvn org.sonarsource.scanner.maven:sonar-maven-plugin:3.7.0.1746:sonar\''
        }

      }
    }

  }
}