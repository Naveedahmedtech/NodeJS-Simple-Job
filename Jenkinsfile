pipeline {
    agent any 
    tools { 
        nodejs "nodeJS"  
    }
    stages {
        stage('Example') {
            steps {
                bat 'npm version'
            }
        }
    }
}
