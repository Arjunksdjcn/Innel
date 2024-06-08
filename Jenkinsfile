pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Checkout code from Git
                git 'https://github.com/your-repo/your-project.git'
            }
        }
        stage('Build') {
            steps {
                // Example build step
                sh './gradlew build' // Adjust this line based on your build tool, e.g., mvn for Maven
            }
        }
        stage('Test') {
            steps {
                // Example test step
                sh './gradlew test' // Adjust this line based on your testing framework
            }
        }
        stage('Deploy') {
            steps {
                // Example deploy step
                sh 'echo "Deploying application..."' // Replace this with actual deployment commands
            }
        }
    }

    post {
        success {
            echo 'Pipeline completed successfully!'
        }
        failure {
            echo 'Pipeline failed!'
        }
    }
}
