pipeline {
  agent any
  stages {
    stage('Checkout') {
      steps {
        git branch: 'main', url: 'https://github.com/PriyankaJoshi2/jenkins-demo.git'
      }
    }
    
    stage('Run App') {
      steps {
        sh 'python3 app.py'
      }
    }
  }
}
