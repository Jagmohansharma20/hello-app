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

        stage('Archive'){
            steps {
                archiveArtifacts artifacts: 'target/*.jar'
            }
        }

        stage('Test') {
            steps {
                echo 'Testing...'
            }
        }
        
    }
}