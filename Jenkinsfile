pipeline {
  agent any
  stages {
    stage('error') {
      parallel {
        stage('version') {
          steps {
            sh 'mvn --version'
          }
        }

        stage('') {
          steps {
            sh 'mvn clean test'
          }
        }

      }
    }

  }
}