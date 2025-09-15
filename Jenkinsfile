pipeline {
    agent any

    tools {
        jdk 'JAVA_HOME'
        maven 'Maven-3.6.3'
    }

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/islemmansouri/ExamenFinale.git'
            }
        }

        stage('Build') {
            steps {
                sh 'mvn clean install'
            }
        }
    }
}
