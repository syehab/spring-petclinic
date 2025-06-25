pipeline {
  agent any

  tools {
    maven 'maven-3.9.7'
  }

  stages {
    stage('Build') {
      steps {
        sh 'mvn clean install'
      }
    }

    stage('Test') {
      steps {
        sh 'mvn test'
      }
    }

    stage('Package') {
      steps {
        sh 'mvn package'
      }
    }
  }
}
