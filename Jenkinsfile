pipeline {
    agent { docker { image '127.0.0.1:32000/python:3.5.1' } }
    stages {
        stage('build') {
            steps {
                sh 'python --version'
            }
        }
    }
}
