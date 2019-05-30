pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                sh 'echo "do some maven magic"'
            }
        }
        stage('Verify') { 
            steps {
                sh 'echo "scan image with tag latest"'
            }
        }
        stage('Deploy to staging env') { 
            steps {
            	sh 'echo "deploy staging..."'
            }
        }
        stage('Deploy to production env') { 
            steps {
            	sh 'echo "deploy production..."'
            }
        }
    }
}
