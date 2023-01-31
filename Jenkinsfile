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
                sh 'npm install -g cnpm --registry=https://registry.npm.taobao.org'
                sh 'cnpm install'
            }
        }
    }
}