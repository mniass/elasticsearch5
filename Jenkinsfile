pipeline {
    agent any
    stages {
      stage('Build') {
         steps {
           sh 'docker build -t elasticsearch:5.6.3 .'
         }
      }
    } 
}
