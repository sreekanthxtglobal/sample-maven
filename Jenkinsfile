pipeline {
    agent any
    //Another option for adding failfast is adding an option to the pipeline definition: parallelsAlwaysFailFast().
     options {
        parallelsAlwaysFailFast()
    }
    stages {
        stage('Non-Parallel Stage') {
            steps {
                echo 'This stage will be executed first.'
            }
        }
        stage('Parallel Stage') {
            when {
                branch 'bugfix'
            }
            
            parallel {
                stage('Branch A') {
                    
                    steps {
                        echo "On Branch A"
                    }
                }
                stage('Branch B') {
                    
                    steps {
                        echo "On Branch B"
                    }
                }
                stage('Branch C') {
                  
                    stages {
                        stage('Nested 1') {
                            steps {
                                echo "In stage Nested 1 within Branch C"
                            }
                        }
                        stage('Nested 2') {
                            steps {
                                echo "In stage Nested 2 within Branch C"
                            }
                        }
                    }
                }
            }
        }
    }
}
