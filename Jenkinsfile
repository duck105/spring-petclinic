pipeline {
  agent any
  stages {
    stage('SonarQube') {
      steps {
        withSonarQubeEnv('sonar_server') {
          sh 'echo "hahaha"'
        }

      }
    }

  }
}