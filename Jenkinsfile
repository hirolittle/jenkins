pipeline {
    agent any

    tools {
        maven 'mvn-3.8.6'
    }

    stages {
        stage('build') {
            steps {
                sh "mvn clean package spring-boot:repackage"
                sh "printenv"
            }
        }
    }
}