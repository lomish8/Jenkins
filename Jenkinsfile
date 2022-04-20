pipeline {
  agent any
  stages {
    stage('error') {
      parallel {
        stage('version') {
          steps {
            bat 'mvn --version'
          }
        }

        stage('errora') {
          steps {
            bat 'mvn clean test'
          }
        }

        stage('a') {
          steps {
            sh 'mvn --vesrion'
          }
        }

      }
    }

  }
  tools {
    maven 'MAVEN_HOME'
  }
}
