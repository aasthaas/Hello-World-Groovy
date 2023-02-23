pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Checkout code from Git repository
                git branch: 'main', url: 'https://github.com/aasthaas/Hello-World-Groovy'
            }
        }

        stage('Build') {
            steps {
                // Build code using Maven
                sh 'mvn clean install'
            }
        }

        stage('Test') {
            steps {
                // Run unit tests using Maven
                sh 'mvn test'
            }
        }
    }
}
