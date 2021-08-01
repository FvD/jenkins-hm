pipeline {
    agent any
    environment {
        CI = 'true' 
        HOME = '.'
    }
    stages {
        stage('Build Container') { 
            steps {
                sh 'docker build -t test-app:${BUILD_NUMBER} . ' 
            }
        }
    }
}
