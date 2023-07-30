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
                    "${env.BRANCH_NAME}" ==~/(1-pipeline | main)/
                }
            } 

        }
        steps{
              echo "executed master stage"

        }
    }
}



}
