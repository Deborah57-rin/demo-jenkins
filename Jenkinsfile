pipeline {
  agent any
  stages {
    stage('Checkout') { steps { checkout scm } }
    stage('Build') {
      steps {
        echo 'Build: show files'
        sh 'ls -la'
      }
    }
    stage('Test') {
      steps {
        echo 'No tests for demo — replace with real test commands'
      }
    }
  }
  post { always { archiveArtifacts artifacts: '**/*', fingerprint: true } }
}
