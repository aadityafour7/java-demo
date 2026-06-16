pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git 'https://github.com/aadityafour7/java-demo.git'
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