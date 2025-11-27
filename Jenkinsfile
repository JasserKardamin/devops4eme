pipeline {
    agent any
    stages {
        stage('Build') {
            sh 'mvn clean install'
        }
        stage('Test') {
            sh 'mvn test'
        }
        stage('Deploy') {
            sh 'echo "Deploying..."'
        }
    }
}
