def myparams = ""
pipeline {
    agent any
    
    parameters {
        string(name: 'Number_of_Clients', defaultValue: '1', description: 'Total number of client')
    }
    stages {
        stage('jenkins home') {
            steps {
                script{
                    for(int i = 0 ; i < "${paras.Number_of_Clients}" ; i++){
                             echo "${paras.Number_of_Clients}"
                    }
                }
            }
        }
    }
}
