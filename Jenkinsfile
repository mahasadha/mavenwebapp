pipeline {
    agent any

    environment {
    PATH = "C:\\WINDOWS\\SYSTEM32; C:\\Users\\vignesh\\apache-maven-3.9.6\\bin"
    }

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
