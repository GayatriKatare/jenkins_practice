def myfile = ""
pipeline {
    agent any
    
   parameters {
        file(name: 'data', description: 'Data file')
    }
    stages {
        stage('jenkins home') {
            steps {
                script{
                    myfile = readFile(file: "${params.data}")
                     echo "${myfile}"
                    }
            }}
}}
