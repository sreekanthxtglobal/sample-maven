pipeline{
agent any
environment{
    COURSE="TIBCO"
}
stages{

    failFast true
    stage("Master"){
        parallel{
         stage("parallel 1"){
            steps{
                echo "executed parallel 1 stage  ${env.BRANCH_NAME}"
                sleep 30
          }
            
         }
         stage("parallel 2"){
            steps{
                echo "executed parallel 2 stage  ${env.BRANCH_NAME}"
          
          }
            
         }
         stage("parallel 3"){
            steps{
                echo "executed parallel 3 stage  ${env.BRANCH_NAME}"
            
          }
            
         }
         
        }
        
    }
     stage("BranchName"){
         steps{
            echo "executed master stage  ${env.BRANCH_NAME}"
        }
            
    }


}
}
