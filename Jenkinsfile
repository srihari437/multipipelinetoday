pipeline {
   agent any
   tools {
      jdk "javah"
      maven "mavenh"
  }
   stages {
     stage ('git checkout') {
           steps {
               git 'https://github.com/srihari437/multipipelinetoday.git'
           }
       }
     stage ('build') {
          steps {
                sh 'mvn clean package'
          }
      }       
     stage ('deploy') {
           steps{
               sh '/opt/shell.sh'
           }
       }         
   }  
}
