pipeline {
    agent any 

    tools {
        nodejs 'nodeJS'  
    }

    stages {
        stage('Checkout Code') {
            steps {
                // Clones the repository
                git branch: 'master', url: 'git@github.com:Naveedahmedtech/NodeJS-Simple-Job.git'
            }
        }

        stage('Install Dependencies') {
            steps {
                // Install npm dependencies
                bat 'npm install'
            }
        }

        stage('Run Tests') {
            steps {
                // Run your tests
                bat 'npm version'
            }
        }

        stage('Build Application') {
            steps {
                // Build the application (if applicable)
                bat 'npm version'
            }
        }
    }

    post {
        always {
            // Archive the build artifacts (optional)
            archiveArtifacts artifacts: '**/build/**/*', allowEmptyArchive: true
        }
    }
}
