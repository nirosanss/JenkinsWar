pipeline {
  agent {
    node {
      label 'master'
    }

  }
  stages {
    stage('build') {
      steps {
        echo 'Start Build'
        bat 'mvn --version'
      }
    }
    stage('SIT') {
      steps {
        echo 'Deployment to SIT'
      }
    }
  }
}