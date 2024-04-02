pipeline {
    agent any

    environment {
    PATH = "C:\\WINDOWS\\SYSTEM32; C:\\Users\\vignesh\\apache-maven-3.9.6\\bin"
    set JAVA_HOME='C:\\Program Files\\Java\\jdk-17'
    }

    stages {
        stage('connect') {
            steps {
                git branch:'main' , url: 'https://github.com/mahasadha/mavenwebapp.git'
            }
        }
        stage('build') {
            steps {
                set JAVA_HOME='C:\\Program Files\\Java\\jdk-17'
                bat 'C:\\Users\\vignesh\\apache-maven-3.9.6\\bin\\mvn clean'
            }
        }
        stage('test') {
            steps {
                set JAVA_HOME='C:\\Program Files\\Java\\jdk-17'
                bat 'C:\\Users\\vignesh\\apache-maven-3.9.6\\bin\\mvn test'
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
