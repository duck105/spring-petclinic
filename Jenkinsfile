pipeline {
  agent any
  stages {
    stage('SonarQube') {
      steps {
        withSonarQubeEnv('sonar_server') {
          sh 'sh \'./mvnw clean package sonar:sonar\''
        }

      }
    }

  }
}