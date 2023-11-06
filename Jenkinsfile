
pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Checkout your source code from version control (e.g., Git)
                checkout scm
            }
        }
        stage('Build') {
            steps {
                // Build your Spring Boot application
                sh 'mvn clean install'
            }
        }
        stage('Unit Tests') {
            steps {
                // Run unit tests here
                sh 'mvn test'  // Adjust the command for your project and build tool
            }
        }
        // Add more stages for deployment or integration testing as needed
    }

    post {
        // Add post-build actions if necessary
    }
}
