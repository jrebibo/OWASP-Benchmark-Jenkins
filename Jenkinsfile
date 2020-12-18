pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo "Building..."
                withMaven {
                    sh "mvn clean verify"
                    sh "mvn compile"
                }
            }
        }
    }
}