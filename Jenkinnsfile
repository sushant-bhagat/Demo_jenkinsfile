pipeline{
    
  agent any
  
  tools{
      maven 'mymaven'
  }
  
  stages{
      stage('checkout code')
      {
         steps{
           git 'https://github.com/Sonal0409/DevOpsCodeDemo.git'
         }
      }
      stage('compile code')
      {
          steps{
              sh 'mvn compile'
          }
  }
      stage('test code')
      { 
          steps{
              sh 'mvn test'
          }
}
      stage('buid code')
      {
          steps{
              sh 'mvn clean install package'
          }
      }
  }
  
}
