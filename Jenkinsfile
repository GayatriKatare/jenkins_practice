def myfile = ""
pipeline {
    agent {label 'cli'}
    
    stages {
        stage('jenkins home') {
            steps {
                script{
                    sh "aws configure"
                    }
            }}
}}
