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
        sh 'apt-get update'
        sh 'apt-get install -y python3'
        sh 'python3 app.py'
      }
    }
  }
}
