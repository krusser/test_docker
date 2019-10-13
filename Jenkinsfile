peline {
    agent {
        docker {
            image 'nginx:latest'
            args '-p 80:80'
        }
    }
    stages {
        stage('Build') {
            steps {
                sh 'docker ps'
            }
        }
    }
}

