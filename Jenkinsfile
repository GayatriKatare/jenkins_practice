pipeline {
    agent any
    
    stages {
        stage('jenkins home') {
            steps {
                
                    sh """
                     cd ${WORKSPACE}
                     mkdir clients_attributes && cd clients_attributes
                     touch data.txt
                     aws configure set aws_access_key_id ""
                     aws configure set aws_secret_access_key ""
                     aws configure set default.region "us-east-1"
                     aws secretsmanager get-secret-value --secret-id secrets --query SecretString --output text >> data.txt
                     """
                 
            }}
}}
