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
                     myfile = readFile('data.txt')
                     echo "${myfile}"
                    }
            }}
}}
