pipeline {
    agent any
    stages {
        stage('Hello') {
            steps {
                echo 'Hello World!'
            }
        } 
        stage('cat ReadMe') {
            when 
            {
            branch "dev"
            }
            steps {        
               script {
                    url = sh (script: 'cat README.md',returnStdout: true).trim()
                    sh """
                      echo ${url}
                      """
                   }
            }    
        }
    }
}
