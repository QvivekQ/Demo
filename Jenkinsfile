pipeline {
    agent any
    tools 'maven 3.3.9'

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                sh 'mvn clean'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                sh 'mvn test'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
                sh 'mvn deploy'
            }
        }
    }
}
