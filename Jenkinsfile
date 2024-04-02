pipeline {
    agent any

    stages {
        stage('connect') {
            steps {
                git branch:'main' , url: 'https://github.com/mahasadha/mavenwebapp.git'
            }
        }
        stage('build') {
            steps {
                bat 'mvn clean'
            }
        }
        stage('test') {
            steps {
                bat 'mvn test'
            }
        }
        stage('deploy') {
            steps {
                //deploy success
                echo 'deploy'
            }
        }
    }
    
}
