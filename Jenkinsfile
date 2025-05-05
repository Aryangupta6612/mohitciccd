pipeline {
  agent any

  stages {
    stage('Pull Node Image') {
      steps {
        sh 'docker pull node:16-alpine'
      }
    }

    stage('Run Node Version Check') {
      steps {
        sh 'docker run -d node:16-alpine node --version'
      }
    }
  }
}
