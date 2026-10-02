pipeline {
    agent any
    tools {
        maven 'Maven 3.9' // Matches the name configured in Jenkins Tools
    }
    stages {
        stage('Build') {
            steps {
                bat 'mvn clean compile'
            }
        }
        stage('Test') {
            steps {
                bat 'mvn test'
            }
        }
    }
    post {
        success {
            echo 'BUILD SUCCESSFUL!'
        }
        failure {
            echo 'BUILD FAILED!'
        }
    }
}
