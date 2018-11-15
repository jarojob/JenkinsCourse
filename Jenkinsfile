node {
  checkout scm
  stage('Build') {
      echo 'Building....' 
      sh 'mvn compile'
   
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
