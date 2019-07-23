pipeline {
  agent {
    docker {
      image 'node:6-alpine'
      args '-p 3000:3000 -p 5000:5000'
    }
  }
  environment {
    CI = 'true'
  }
  stages {
    stage('Build'){
      steps {

      }
    }
    stage('Test'){
    steps {

      }
    }
    stage('Deliver for development'){
      when {
        branch 'Development'
      }
      steps {
        sh './jenkins/scripts/deliver-for-development.sh'
      }
    }
  }
}
