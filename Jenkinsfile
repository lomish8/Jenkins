pipeline {
  agent any
  stages {
    stage('error') {
      parallel {
        stage('Version Check') {
          steps {
            bat 'mvn --version'
          }
        }

        stage('Run Project') {
          steps {
            bat 'mvn clean test'
          }
        }

      }
    }

  }
  tools {
    maven 'MAVEN_HOME'
  }
}