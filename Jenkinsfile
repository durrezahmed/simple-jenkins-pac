pipeline {
    agent any
    stages {
        stage('Fetch Code') {
            steps {
                git url: 'https://github.com/durrezahmed/vprofile-project-devops'
            }
        }

        stage('Build') {
            steps {
                sh 'mvn install'
            }
        }

        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }
    }
}