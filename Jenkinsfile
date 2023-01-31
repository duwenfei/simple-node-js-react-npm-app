pipeline {
    agent {
        docker {
            image 'node:lts-bullseye-slim'
            args '-p 3000:3000'
        }
    }
    stages {
        stage('Build') {
            steps {
                sh 'npm cache clean --force && npm config rm proxy && npm config rm https-proxy && npm cache verify && npm install'
            }
        }
    }
}