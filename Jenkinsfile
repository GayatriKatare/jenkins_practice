def myparams = ""
int data = 0
pipeline {
    agent any
    
    parameters {
        string(name: 'Number_of_Clients', defaultValue: '1', description: 'Total number of client')
    }
    stages {
        stage('jenkins home') {
            steps {
                script{
                    data = "${paras.Number_of_Clients}" 
                    for(int i = 0; i < data; i++){
                             build job: 'PARAM_TEST1', parameters: [string(name: 'MYPARAM', value: "${params.MYPARAM}")]
                    }
                }
            }
        }
    }
}
