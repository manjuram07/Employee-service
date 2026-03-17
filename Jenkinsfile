pipeline {
    agent any

    stages {

        stage('Clone Code') {
            steps {
                git 'https://github.com/manjuram07/Employee-service.git'
            }
        }

        stage('Build') {
            steps {
                sh 'mvn clean install'
            }
        }

        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }

    }
}