#!/usr/bin/env groovy
node {
  checkout scm
  stage('Build') {
      echo 'Building....' 
      withMaven(
        maven:'Maven Test'
      ) {
        sh 'mvn compile'
      }
   }
  stage('Test') {
       echo 'Testinging....' 
       sh 'mvn test'
 
   }
  stage('Deploy') {
     echo 'Deploying....'
     sh 'mvn package'
     }
  
}
