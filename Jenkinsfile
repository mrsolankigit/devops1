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
                      echo "Readme file changed inside dev branch only" 
                      bat 'echo "Hello from dev branch!"'     
                      sh 'echo "Hi"'
            }    
        }
    }
}
