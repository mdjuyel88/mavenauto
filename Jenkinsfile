pipeline {
  agent {
    node {
      label 'master'
    }

  }
  stages {
    stage('compile') {
      steps {
        sh 'mvn compile'
      }
    }

    stage('package') {
      steps {
        sh 'mvn package'
      }
    }

    stage('install') {
      steps {
        sh 'mvn install'
      }
    }

  }
}