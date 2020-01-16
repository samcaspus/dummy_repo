pipeline {
   agent any

   stages {
      stage('clone') {
      steps{
         sh 'pwd'
         sh 'rm -rf dummy_repo'
         sh 'git clone https://github.com/samcaspus/dummy_repo.git'
         sh 'pwd'
      }
      }
      stage('unpack') {
          steps{
         sh 'cd dummy_repo && javac main.java'
      }
      }
      stage('execute') {
       steps{
         
          sh 'cd dummy_repo && java main'
      }
      }
      
      
   }
}
