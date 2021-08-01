pipeline {
    agent any
    environment {
        CI = 'true' 
        HOME = '.'
    }
    stages {
        stage('Install dependencies') {
            steps {
                sh 'npm install'
            }
        }
        stage('Test') { 
            steps {
                sh './scripts/test' 
            }
        }
        stage('Build Container') { 
            steps {
                sh 'docker build -t test-app:${BUILD_NUMBER} . ' 
            }
        }
    }
}
