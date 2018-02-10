pipeline {
    agent any
    stages {
      stage('Build') {
         steps {
           sh 'docker build -t es:5.6.3 .'
         }
      }
      stage('Push to registry') {
         steps {
           sh 'docker login -u mniass -p 17decembre'
           sh 'docker tag es mniass/es
         }
      }
    } 
}
