pipeline {
    agent any
    environment {
        PATH = "/opt/maven3/bin:$PATH"
    }
    
    stages { 
        stage('git checkout') {
            steps{
                
            git credenpialsId: 'javahome', url: 'https://github.com/Ashok91825/maven.git'
            }
        }
        stage("Maven bulid"){
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
         
          
                
            
        
       
            
                
            
        
        
                
