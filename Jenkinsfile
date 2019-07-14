pipeline {
    agent any
    stages {
        stage('Clean and CLone') {
            steps {
                sh "rm -rf sample-boot-jenkins"
                sh "git clone https://github.com/Sri2614/sample-boot-jenkins.git"
                sh "mvn clean -f sample-boot-jenkins"
            }
        }
        stage('Install') {
            steps {
                sh "mvn install -f sample-boot-jenkins"
            }
        }
        stage('Test') {
            steps {
                sh "mvn test -f sample-boot-jenkins"
            }
        }
        stage('Example package') {
            steps {
                sh "mvn package -f sample-boot-jenkins"
            }
        }
    }
}

