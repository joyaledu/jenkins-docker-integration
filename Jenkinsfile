pipeline {
    agent {
        docker {
            image 'alpine:latest'
            // Run the container on the node specified at the
            // top-level of the Pipeline, in the same workspace,
            // rather than on a new node entirely:
            reuseNode true
        }
    }
    stages {
        stage('Build') {

            steps {
                echo 'Building..'
                sh 'ls'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                sh 'cat /proc/uptime'
                sh 'cat /proc/cpuinfo'
                sh 'cat /proc/meminfo'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
