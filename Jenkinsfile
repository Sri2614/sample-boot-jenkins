pipeline {
    agent any
    tools {
        maven 'Maven3.6.1'
        jdk 'JDK1.8'
    }
    stages {
        stage ('Initialize') {
            steps {
                sh '''
                    echo "PATH = ${PATH}"
                    echo "M2_HOME = ${M2_HOME}"
                '''
            }
        }

        stage ('Build') {
            steps {
                sh 'mvn install' 
            }
            
        }
    }
}
