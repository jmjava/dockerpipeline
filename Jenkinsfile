pipeline {
    agent { label 'java-mvn-docker' }
    stages {
        stage('Test') {            
            steps {
                sh 'sudo docker build .'               
            }
        }
    }
}

