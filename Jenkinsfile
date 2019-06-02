pipeline {
    agent { label 'java-mvn-docker' }
    stages {
        stage('Test') {
            agent { dockerfile true }
            steps {
                sh 'node --version'
                sh 'svn --version'
            }
        }
    }
}

