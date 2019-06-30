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
        bat 'mvn clean package'
      }
    }
    stage('Packaging') {
      steps {
        echo 'Prepare Package'
        archiveArtifacts 'target/*.war'
      }
    }
    stage('SIT') {
      steps {
        echo 'Deployment to SIT'
      }
    }
  }
}