def myfile = ""
pipeline {
    agent any
    
   parameters {
        file(name: 'data', file: 'data.txt', description: 'Data file')
    }
    stages {
        stage('jenkins home') {
            steps {
                script{
                    sh "mv data1 ${params.data}"
                    myfile = readFile(file: "${params.data}")
                     echo "${myfile}"
                    }
            }}
}}
