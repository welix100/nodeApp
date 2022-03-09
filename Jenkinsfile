pipeline {
  agent any

  environment {
    PATH = "/home/worker/.nvm/versions/node/v16.4.0/bin:${env.PATH}"
  }

  stages {

    stage('Install Dependencies') {
      steps {
        sh 'npm install'
      }
    }

    stage('Test') {
      steps {
        sh 'npm run test'
      }
    }
    
    stage('Publish') {
      steps {
        echo 'publish'
      }
    }
  }
}
