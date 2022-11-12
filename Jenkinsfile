pipeline {
    agent any
    stages {
        stage ("Pull") {
            steps{
                script{
                    checkout([$class: 'GitSCM', branches: [[name: '*/master']],
                    userRemoteConfigs: [[
                        credentialsId: 'github', 
                        url: 'https://github.com/hiba-khalfaoui/Project_LC.git' ]]])
                }
            }
        }
        
         stage('python test'){
            steps{
                script{
                    sh "python3 --version"
                }
            }
        }
        stage('Build'){
            steps{
                script{
                    sh "ansible-playbook Ansible/build.yml -i Ansible/inventory/host.yml -e ansible_become_password=123"
                }
            }
        }
  
  
  
  
  
  
  
  }
}
