pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                echo 'Cloning done'
            }
        }

        stage('Build') {
            steps {
                bat 'mvn clean install'
            }
        }

        stage('Test') {
            steps {
                echo 'Testing...'
            }
        }
    }
}
