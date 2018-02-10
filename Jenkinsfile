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
           sh 'docker tag es:5.6.3 mniass/es:5.6.3'
           sh 'docker push  mniass/es:5.6.3'
         }
      }
    } 
}
