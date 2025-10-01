pipeline {
  agent {
        docker {
            image 'python:3.9'
        }
    }
  stages {
    stage('Checkout') {
      steps {
        checkout scm
      }
    }
    stage('Build') {
      steps {
        echo 'Building the project...'
        sh 'pip install -r requirements.txt || true'
       
      }
    }
    stage('Test') {
      steps {
        echo 'Running tests... (simulated)'
        sh 'pytest || exit 1'
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
