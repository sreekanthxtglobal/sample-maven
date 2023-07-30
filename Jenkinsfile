ipeline{
    agent any
    tools{
        maven "mvn_autoinstaller"
    }
    stages{
        stage("maven autoinstaller"){
           
            steps{
                script{
                    echo " maven version "
                    sh 'mvn -version'
                }
            }
            
        }
         stage("jdk17"){
            tools{
                jdk 'java17.0.2'
            }
            steps{
                script{
                    echo " maven version "
                    sh 'mvn -version'
                }
            }
            
        }
    }

       
    
}
