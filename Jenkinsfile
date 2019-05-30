pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'echo "do some maven magic"'
        sh 'echo "something like mvn fat-jar"'
      }
    }
    stage('Verify') {
      steps {
        sh 'echo "scan image with tag latest"'
      }
    }
    stage('Deploy to staging env') {
      steps {
        input 'rly?'
        sh 'echo "deploy staging..."'
      }
    }
    stage('Deploy to production env') {
      steps {
        input 'rly?'
        sh 'echo "deploy production..."'
      }
    }
  }
}