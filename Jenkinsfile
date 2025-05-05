pipeline {
  agent any

  stages {
    stage('Pull Node Image') {
      steps {
        bat 'docker pull node:16-alpine'
      }
    }

    stage('Run Node Version Check') {
      steps {
        bat 'docker run -d node:16-alpine node --version'
      }
    }
  }
}
