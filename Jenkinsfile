pipeline {
    agent { label 'java-mvn-docker' }
    stages {
        stage('Build Docker image') {            
            steps {
                sh 'sudo docker build -t sample .'   
                sh 'sudo docker tag sample gcr.io/jmrhattrain/sample:version1.0'
                sh 'sudo docker push gcr.io/jmrhattrain/sample:version1.0'
              
            }
        }
    }
}

