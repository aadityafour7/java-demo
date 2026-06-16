pipeline {
    agent any

    stages {

        stage('Environment') {
            steps {
                bat 'java -version'
                bat '.\\mvnw.cmd -version'
            }
        }

        stage('Build') {
            steps {
                bat '.\\mvnw.cmd clean compile'
            }
        }

        stage('Test') {
            steps {
                bat '.\\mvnw.cmd test'
            }
        }

        stage('Package') {
            steps {
                bat '.\\mvnw.cmd package'
            }
        }
    }
}