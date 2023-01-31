pipeline {
    agent {
        docker {
            image 'hbrls/cnpmjs:latest'
            args '-p 3000:3000'
        }
    }
    stages {
        stage('Build') {
            steps {
                sh 'cnpm install'
            }
        }
    }
}