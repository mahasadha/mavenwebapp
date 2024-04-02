pipeline {
    agent any

    stages {
        stage('connect') {
            steps {
                git 'https://github.com/mahasadha/mavenwebapp.git'
            }
        }
        stage('build') {
            steps {
                sh 'mvn clean'
            }
        }
        stage('test') {
            steps {
                sh 'mvn test'
            }
        }
        stage('deploy') {
            steps {
                echo 'deploy successful'
            }
        }
    }
    
}