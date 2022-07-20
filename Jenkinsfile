pipeline {
    agent any

    stages {
        stage('changeset condition') {
            when {
        changeset "example.txt";
        anyOf {
          branch "main";
          branch "test";
          branch "master";
        }
      }
      steps {
        echo "++++It's Working++++"
      }
        }
    }
}
