pipeline {
  agent any
  stages {
    stage('Preparation') {
      steps {
        git 'https://github.com/spring-projects/spring-petclinic.git'
      }
    }

    stage('Build') {
      steps {
        sh './mvnw package'
      }
    }

  }
}