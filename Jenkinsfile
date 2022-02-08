pipeline {
    agent any
    environment {
        PATH = "/opt/maven3/bin:$PATH"
    }
    
    stages { 
        stage('git checkout') {
            steps{
                
            git credentialsId: 'javahome' ; url: 'https://github.com/Ashok91825/maven.git'
            }
        }
        stage("Maven Bulid"){
            steps{
                sh "mvn clean package"
            }
        }
        stage("deploy-dev") {
            steps{
                sshagent(['name']) {
                }
            }
        }
    }
}
         
          
                
            
        
       
            
                
            
        
        
                
