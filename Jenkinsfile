pipeline {
   agent {
       docker {
           image 'node:10'
       }
   }
   environment {
       CI = 'true'
   }
   stages {
       stage('Build') {
           steps {
               sh 'node --version'
               sh 'npm install'
           }
       }
   }
}