def myfile = ""
pipeline {
    agent any
    
    parameters {
        file(name: 'data.txt', description: 'Data file')
    }
    stages {
        stage('jenkins home') {
            steps {
                script{
                    myfile = readFile(file: "F:/Devops/Terraform/AWS/data.txt")
                     echo "${myfile}"
                    }
            }}
}}
