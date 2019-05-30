pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                sh 'echo do some maven magic'
            }
        }
        stage('Verify') { 
            steps {
                sh 'scan image with tag latest'
            }
        }
        stage('Deploy to staging env') { 
            steps {
            	sh 'deploy staging...'
            }
        }
        stage('Deploy to production env') { 
            steps {
            	sh 'deploy production...'
            }
        }
    }
}
