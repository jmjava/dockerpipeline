pipeline {
    agent { label 'java-mvn-docker' }
    stages {
        stage('Build Docker image') {            
            steps {
                sh 'sudo docker build .'   
                sh 'sudo docker docker tag sample gcr.io/jmrhattrain/sample:version1.0'
                sh 'sudo docker push gcr.io/jmrhattrain/sample:version1.0'
              
            }
        }
    }
}

