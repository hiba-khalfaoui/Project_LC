pipeline
{
  agent any
  stages{
    stage('pull'){
     steps{
      scripts{
           checkout([$class: 'GitSCM' , branches: [[name: '*/master']],
             userRemoteConfigs: [[
                   credentialsId: 'github', url: 'https://github.com/hiba-khalfaoui/Project_LC.git' ]]])
                      
          }
         }
        }
    
  
  
  
  
  
  
  
  
  }
}
