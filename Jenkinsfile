pipeline {
    agent any
    tools {
        maven 'Maven_3.8'
    }
    stages {
        stage('Build') {
            steps {
                echo "Building..."
                sh 'mvn -B -DskipTests clean package'
            }
        }
        stage('Test') {
            steps {
                sh "mvn clean verify"
            }
        }
    }
}