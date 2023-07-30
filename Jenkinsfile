pipeline{
agent any
environment{
    COURSE="TIBCO"
    
}
stages{
    stage("Master"){
        when{
            allOf{

                environment name: "COURSE" , value: "TIBCO"
                expression {
                    env.BRANCH_NAME ==~/(main|bugfix|dev)/
                }
            } 
        }
        steps{
              echo "executed master stage"
        }
    }
      stage("BranchName"){
         steps{
            echo "executed master stage  ${env.BRANCH_NAME}"
        }
            
    }


}
}
