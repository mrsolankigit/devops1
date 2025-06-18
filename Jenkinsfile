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
                cat README.md
            }    
        }
    }
}
