pipeline {
    agent any
    environment {
        MAVEN_HOME = 'C:\\Program Files\\apache-maven-3.9.7' // Adjust this path according to your Maven installation directory on Windows
        PATH = "${env.PATH};${env.MAVEN_HOME}\\bin"
    }
    stages {
        stage('Build') {
            steps {
                bat 'mvn clean'
            }
        }
        stage('Test') {
            steps {
                bat 'mvn test'
            }
        }
    }
}
