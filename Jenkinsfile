pipeline
{
  agent any
  stages{
    stage('pull'){
     steps{
      scripts{
           checkout([$class: 'GitSCM' , branches: [[name: '*/master']],
             userRemoteConfigs: [[
                      credentialsId: '4044e336-7809-4dfa-aaa5-3b0d95e13af5',
                      url: 'https://github.com/hiba-khalfaoui/Project_LC.git']]])
                      
          }
         }
        }
    }
}
