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
                sh 'FLASK_ENV=development FLASK_APP=main.py flask run'
            }
        }
    }
}
