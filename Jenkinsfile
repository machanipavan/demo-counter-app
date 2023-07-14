pipeline{
    
    agent any 
    
    stages {
        
        stage('Git Checkout'){
            
            steps{
                
                script{
                  git branch: 'main', credentialsId: 'nani', url: 'https://github.com/sushmireddy05/demo-counter-app.git'
                }
            }
        }
      
        stage('UNIT testing'){
            
            steps{
                
                script{
                    
                    sh 'mvn test'
                }
            }
        }
    }
}