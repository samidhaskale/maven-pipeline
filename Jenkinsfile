pipeline {
    agent { label 'slaveNode1' }

    tools {
        maven 'maven'
        jdk 'jdk17'
    }

    stages {

        stage('Checkout') {
            steps {
                git 'https://github.com/your-repo/maven-pipeline.git'
            }
        }

        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }

        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }

    }
}
