pipeline {
    agent any
    stages {
        stage('git') {
            steps {
                sh "git --version"
            }
        }
        stage('mvn') {
            steps {
                sh "mvn --version"
            }
        }
    }
} 
