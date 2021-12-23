pipeline {
    agent cli
    
    parameters {
        string(name: 'Number_of_Clients', defaultValue: '1', description: 'Total number of client')
    }
    stages {
        stage('jenkins home') {
            steps {
                Sript{
                    for(int i = 0; i < ${paras.Number_of_Clients}; i++){
                    def myparams = string(name: 'MYPARAM', value: "${params.MYPARAM}")
                    build job: 'downstream-pipeline-with-params', parameters: myparams
                    }
                }
            }
        }
    }
}
