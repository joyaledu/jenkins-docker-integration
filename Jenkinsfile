pipeline {
    agent {
        docker { image 'node:16.13.1-alpine' }
    }
    stages {
        stage('Testing node') {
            steps {
                sh 'node --version'
                sh 'npm --version'
            }
        }
        stage('Installing vue.js') {
            steps {
                sh 'npm init vue@latest'
            }
        }
    }
}
