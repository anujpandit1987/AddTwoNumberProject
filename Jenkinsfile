pipeline { 
    agent any  
    stages { 
         stage('SCM Checkout') { 
            steps { 
                           echo 'print SCM Checkout'
                
            }
        }
         stage('Build Test') { 
            steps { 
                    mvn 'clean test' 
            }
        }
        stage('Package') { 
            steps { 
                    echo 'This is a minimal pipeline.' 
            }
        }
    }
}
