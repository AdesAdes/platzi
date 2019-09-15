pipeline {
  agent any
  tools {
    nodejs '12.7.0'
  }

  options {
    timeout(time: 2, unit: 'MINUTES')
  }

  stages {
    stage('Install dependencies') {
      steps {
        bat 'npm install'
      }
    }
    stage('Run tests') {
      steps {
        bat 'npm test'
      }
    }
  }
}
