pipeline{
    agent any
    tools{
        maven "mvn_autoinstaller"
    }
    stages{
        stage("satege 1"){
            steps{
                script{
                    echo " maven version stage"
                    sh 'mvn -version'
                }
            }
            
        }
    }
}
