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
        //sh 'pip install -r requirements.txt || true'
        sh 'pip --version || echo "pip not installed"'
       
      }
    }
    stage('Test') {
      steps {
        echo 'Running tests... (simulated)'
        //sh 'pytest || exit 1'
        //sh 'echo "All tests passed!"'
        sh 'exit 1'
      }
    }
    stage('Deploy') {
      steps {
        echo 'Deploying... (simulated)'
        sh 'echo "Application deployed successfully!"'
      }
    }
  }
}
