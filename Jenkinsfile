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
       stage('Install') {
           steps {
               sh 'node --version'
               sh "echo ------- MOBILE APP -------"
               sh 'npm install'
           }
       }
       stage('Test') {
           steps {
               sh 'npm test'
           }
       }
   }
}