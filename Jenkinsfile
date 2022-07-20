pipeline {
    agent any

    stages {
        stage('Hello') {
            when {
        changeset "example.txt";
        anyOf {
          branch "main";
          branch "master";
        }
      }
      steps {
        echo "++++It's Working++++"
      }
        }
    }
}
