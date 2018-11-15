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
    withMaven(
        maven:'Maven Test'
    ) {
       sh 'mvn test'
    }
     
   }
  stage('Deploy') {
     echo 'Deploying....'
    withMaven(
        maven:'Maven Test'
    ) {
     sh 'mvn package'
    }
     }
  
}
