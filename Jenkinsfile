pipeline {
    agent any

    tools {
        maven 'Maven3'
    }

    stages {
        stage('CHECKOUT') {
            steps {
                git 'https://github.com/VarshithaJ07/maven.git'
            }
        }

        stage('Build') {
            steps {
                bat 'mvn clean install'
            }
        }

        stage('Test') {
            steps {
                bat 'mvn test'
            }
        }
    }
}