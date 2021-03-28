pipeline {
  agent any
  stages {
    stage('Cloning Git') {
      steps {
        git 'https://github.com/darshhd/angular-nodejs-docker-compose'
      }
    }
    stage('Docker-compose step') {
      steps{
        script {
          sh "docker-compose down"
          sh "docker-compose up"
        }
      }
    }
  }
}

