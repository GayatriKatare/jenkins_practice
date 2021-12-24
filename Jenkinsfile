def inputFile = ""
pipeline {
    agent any
    
    parameters {
        string(name: 'Number_of_Clients', defaultValue: '1', description: 'Total number of client')
    }
    stages {
        stage('jenkins home') {
            steps {
                script{
                    inputFile = input message: 'Upload file', parameters: [file(name: 'data.txt')]
                    }
            }}
}}
