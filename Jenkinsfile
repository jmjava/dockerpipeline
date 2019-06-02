pipeline {
    agent { label 'java-mvn-docker' }
    stages {
        stage('Build Docker image') {            
            steps {
                sh 'sudo docker build .'               
            }
        }
    }
}

