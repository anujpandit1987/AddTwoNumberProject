pipeline { 
    agent any  
    stages { 
         stage('SCM Checkout') { 
            steps { 
                            git branch: 'main', credentialsId: 'MyGitHubCredentials', url: 'https://github.com/anujpandit1987/AddTwoNumberProject/'
                
            }
        }
        stage('Package') { 
            steps { 
                 def mvnHome= tool name: 'MAVEN_HOME', type: 'maven' 
                sh "${mvnHome}/bin/mvn package"
               echo 'This is a minimal pipeline.' 
            }
        }
    }
}
