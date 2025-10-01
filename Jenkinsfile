pipeline {
  agent any
  stages {
    stage('Checkout') {
      steps {
        checkout scm
      }
    }
    stage('Build') {
      steps {
        echo 'Building the project...'
        sh 'echo "Compiling source code..."'
      }
    }
    stage('Test') {
      steps {
        echo 'Running tests... (simulated)'
      }
    }
    stage('Deploy') {
      steps {
        echo 'Deploying... (simulated)'
      }
    }
  }
}
