pipeline {
  agent {
    docker 'maven:3.3.3'
  }
  stages {
    stage('build') {
      steps {
        bat 'mvn --version'
        echo 'Start Build'
        bat 'mvn clean package'
      }
    }
  }
}