pipeline {
  agent {
    label 'mynode'
  }

  stages {
    stage('Run Test') {
      steps {
        bat "docker-compose up"
      }
    }
    
    stage('Bring Grid Down') {
      steps {
        bat "docker-compose down"
      }
    }
  }
}