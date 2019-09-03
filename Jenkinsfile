pipeline {

    agent any
    
    stages {
        
        stage ('Installing Dependencies') {
           steps {
                sh 'npm install'
                 }
           }
        
        stage ('Testing with Jasmine') {
           steps {
               //sh 'npm install jasmine;'
               echo 'Hello'
               sh 'node_modules/.bin/jasmine'
                 }
           }
      }
}     
