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
              // sh 'node_modules/.bin/jasmine'
               sh 'npm install jasmine-xml-reporter'
               //To run tests, generate a JUnit XML report and place the output in a specific folder:
               sh './node_modules/jasmine-xml-reporter/bin/jasmine.js --junitreport --output=shippable/testresults/'
                 }
           }
      }
}     

