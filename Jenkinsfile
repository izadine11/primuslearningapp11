pipeline {
    agent any
    
    tools {
       git 'git'
       jdk 'JDK'
       maven 'Maven-3.9.9'
    }
    
    stages {
        stage('checking tools version') {
           steps {
      // One or more steps need to be included within the steps block.
              sh 'git -v'
              sh 'java -version'
              sh 'mvn -version'
                 }
             }

        stage('Build') {
           steps {
    // One or more steps need to be included within the steps block.
              sh 'mvn clean'
              sh 'mvn package'
               }
            }
      }
}