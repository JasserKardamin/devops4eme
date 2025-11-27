pipeline {
    agent any

     environment {
           JAVA_HOME = "/usr/lib/jvm/java-21-openjdk-amd64"
           PATH = "${JAVA_HOME}/bin:${env.PATH}"
       }

    stages {
        stage('Build') {
            steps {
                echo 'Building the project...'
                sh 'mvn clean install'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                sh 'mvn test'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying the project...'
                sh 'echo "Deploy step placeholder"'
            }
        }
    }
}
