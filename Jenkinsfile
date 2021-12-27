pipeline {
    agent any
    
    stages {
        stage('jenkins home') {
            steps {
                
                    sh """
                     cd C:/ProgramData/Jenkins/.jenkins/workspace/
                     mkdir clients_attributes && cd clients_attributes
                     touch data.txt
                     curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
                     unzip awscliv2.zip
                     sudo ./aws/install
                     aws --version
                     aws configure set aws_access_key_id "AKIAWEGEGEMYJ7VP6ZUD"
                     aws configure set aws_secret_access_key "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"
                     aws configure set default.region "us-east-1"
                     aws secretsmanager get-secret-value --secret-id secrets --query SecretString --output text > C:/ProgramData/Jenkins/.jenkins/workspace/clients_attributes/data.txt
                     cat C:/ProgramData/Jenkins/.jenkins/workspace/clients_attributes/data.txt
                     """
                 
            }}
}}
