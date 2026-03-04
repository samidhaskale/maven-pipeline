pipeline {
    agent { label 'slaveNode1' }

    tools {
        maven 'maven'
        jdk 'jdk17'
    }

    stages {

        stage('Build') {
            steps {
                bat 'mvn clean package'
            }
        }

        stage('Test') {
            steps {
                bat 'mvn test'
            }
        }

    }
}
