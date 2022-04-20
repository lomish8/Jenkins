pipeline {
  agent any
  stages {
    stage('error') {
      steps {
        sh 'mvn compile test package'
        bat 'mvn clean test'
      }
    }

  }
}