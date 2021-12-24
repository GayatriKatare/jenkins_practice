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
                    myfile = readFile(file: "${params.data.txt}")
                     echo "${myfile}"
                    }
            }}
}}
