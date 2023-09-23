pipeline{
    
    agent any 
    
    stages {
        
        stage('Git Checkout'){
            
            steps{
                
                script{
                    
                    git branch: 'main', url: 'https://github.com/syedaltaf33/demo-counter-app.git'
                }
            }
            
        }
        stage ("UNIT Test"){

            steps{

                script{
                    sh 'mvn test'
                }
            }
        }
        stage ("build test"){

            steps{

                script{
                    sh 'mvn clean install'
                }
            }
        }

    }
        
}
