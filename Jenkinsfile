pipeline {
    agent none 
    stages {
        stage('Build') { 
            agent {
                any {
                    image 'python:2-alpine' 
                }
            }
            steps {
                sh 'export FLASK_ENV=development'
                sh 'export FLASK_APP=main.py'
                sh 'flask run' 
                
            }
        }
    }
}
