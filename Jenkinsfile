pipeline {
    tools{
        jdk 'JAVA_HOME'
        maven 'M2_HOME'
    }
    agent any

    stages {
        
        stage('compile') {
            steps {
                sh 'mvn compile'
            }
        }
        stage('package') {
            steps {
                sh 'mvn package'
            }
        }
        stage('install') {
            steps {
                sh 'mvn install'
            }
        }
    }
}
