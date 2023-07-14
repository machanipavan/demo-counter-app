pipeline{
        
        agent any 
        
        stages {
            
            stage('Git Checkout'){
                
                steps{
                    
                    script{
                    git branch: 'main', url: 'https://github.com/machanipavan/demo-counter-app.git'
                    }
                }

                stage('unit testing')
                    
                    {
                        sh'mvn test'
                    }
                
            }
        
        }
    }
    