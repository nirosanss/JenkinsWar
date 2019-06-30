pipeline {
  agent none
  stages {
    stage('build') {
      steps {
        bat 'mvn --version'
        echo 'Start Build'
        bat 'mvn clean package'
      }
    }
    stage('SIT') {
      steps {
        echo 'Deployment to SIT'
      }
    }
  }
}