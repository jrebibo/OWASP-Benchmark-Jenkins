pipeline {
    agent any
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