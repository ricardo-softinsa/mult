pipeline{
    agent any
    stages{
        /*stage('Git'){
            steps{
                echo "Checking code from repo..."
                //bat "echo Building ${BRANCH_NAME}..."
                
                //Checkout code from the repository
                checkout scm 
            }
        }*/ 
        stage('SonarQube - Analysis'){
            steps{    
                echo "SonarQube Analysis..."
                script{ 
                    echo "SonarQube"                    }
                }  
                
            } 
        
        stage('SonarQube - Quality Gates'){
            steps{    
                echo "Checking Quality Gates..."
            }
        }
        stage('Build'){
            steps{
                echo "Build Application..."
            }
        }
        stage('Deployment'){
            steps{
                echo "Deploying Website..."
                
                
                
            }
        }
    }
    post{
        always{
            deleteDir()
        }
        success{
            echo "Pipeline executed successfully!"
        }
        failure{
            echo "Pipeline failed to execute!"


        }
    }
}
