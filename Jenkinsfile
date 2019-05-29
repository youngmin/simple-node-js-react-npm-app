pipeline {
    agent {
        docker {
            image 'node:8-jessie' 
            args '-p 3000:3000' 
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'cd frontend' 
                sh 'npm install' 
                sh 'npm run build'' 
            }
        }
    }
}
