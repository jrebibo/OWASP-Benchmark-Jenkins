pipeline {
    agent any
    tools {
        maven 'Maven_3.8.0'
    }
    stages {
        stage('Build') {
            steps {
                echo "Building..."
                withMaven {
                    sh 'mvn -B -DskipTests clean package'
                    sh "mvn clean verify"
                }
            }
        }
    }
}