pipeline {
    agent any
    stages {
        stage ('Build') {
            steps {
                sh 'java -version'
                sh 'mvn -version'
                sh 'docker --version'
                
            }
            
        }
      stage('Building image') {
         steps{
            script {
                dockerImage = docker.build registry + ":$BUILD_NUMBER"
        }
      }
    }
    }
}
