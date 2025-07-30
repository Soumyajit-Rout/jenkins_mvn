pipeline {
    //tools {
        
        //maven 'M2_HOME'
   // }
    agent any
    stages {
        stage('checkout') {
            steps {
                git 'https://github.com/Soumyajit-Rout/jenkins_maven_demo.git'
            }
        }
        stage('compile') {
            steps {
                sh 'mvn compile'
            }
        }
       stage('package'){
           steps {
                sh 'mvn package'
            }
        }
       stage('install'){
           steps {
                sh 'mvn install'
            }
        }
    }
}
