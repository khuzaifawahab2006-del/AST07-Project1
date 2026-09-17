pipeline {
    agent any

    parameters {
        choice(
            name: 'ENVIRONMENT',
            choices: ['dev', 'staging', 'prod'],
            description: 'Select the deployment environment'
        )
    }

    stages {

        stage('Checkout') {
            steps {
                git branch: 'main',
                   https://github.com/khuzaifawahab2006-del/AST07-Project1.git
            }
        }

        stage('Show Parameter') {
            steps {
                echo "Selected environment: ${params.ENVIRONMENT}"
            }
        }

        stage('Build for Environment') {
            steps {
                echo "Building the application for the ${params.ENVIRONMENT} environment..."
            }
        }
    }
}
