pipeline {
    agent any  // Runs on any available agent

    environment {
        // Define environment variables if needed
        MY_VAR = 'Some value'
    }

    stages {
        stage('Checkout') {
            steps {
                // Runs a shell command and echoes a message
                sh 'echo "HI GITHUB PIPELINE"'
            }
        }
    }
}
