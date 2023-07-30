pipeline{
agent any

parameters{
    string{
        name: 'LOCATION'
        defaultValue: 'Ameerpet'
    }
}
stages{
    stage("String"){
        steps{
            echo "String parameters ${params.LOCATION}"
        }
    }
}

}
