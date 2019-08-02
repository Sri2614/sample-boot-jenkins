pipeline {
    agent any
    stages {
        stage ('Build') {
            steps {
                sh 'java -version'
                sh 'mvn -version'
                sh 'docker --version'
                sh 'docker pull nginx'
                sh 'docker pull openjdk'
            }
            
        }
     
    }
}
