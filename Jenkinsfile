pipeline {
    agent any  // Runs on any available agent

    environment {
        // Define environment variables if needed
        MY_VAR = 'Some value'
    }

    stages {
        stage('DIRECTORY CONTENTS') {
            steps {
                // Runs a shell command and echoes a message
                sh 'ls -a'
                sh 'echo "THESE FILES CHANGED"'
                sh 'bash db-migration.sh'
            }
        }
        stage('BUILDING') {
            steps {
                // Runs a shell command and echoes a message
                sh 'echo "HI BUILD PIPELINE"'
            }
        }
        stage('DEPLOYINg') {
            steps {
                // Example deploy step
                sh 'echo "HI DEPLOY PIPELINE"'
                // Add your deploy commands here (e.g., kubectl apply, aws deploy, etc.)
            }
        }
    }
}
