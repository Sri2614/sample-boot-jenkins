pipeline {
        agent any

        stages {  
            stage ("first") {
                tools {
                   maven 'Maven3.6.1'
                   jdk "JDK1.8"
         
                }
                steps {
                    sh 'java -version'
                    sh 'mvn -version'
                }
            }
           
       }
      
}
