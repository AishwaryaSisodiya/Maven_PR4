pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git 'https://github.com/AishwaryaSisodiya/Maven_PR4.git'
            }
        }

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

        stage('Package') {
            steps {
                bat 'mvn package'
            }
        }
    }
}
