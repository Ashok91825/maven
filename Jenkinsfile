pipeline {
    agent any 
    stages { 
        stage('git clone') {
            steps{'git branch: 'main', url: 'https://github.com/Ashok91825/maven.git'
            
        stage('Build') { 
            steps {bat 'mvn compile'
                
            }
        }
        stage('Test') { 
            steps {bat 'mvn test'
                
            }
        }
        stage('Deploy') { 
            steps {
                bat 'mvn deploy'
            }
        }
    }
}
