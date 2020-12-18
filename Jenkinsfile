pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo "Building..."
                withMaven {
                    sh "mvn clean verify"
                    sh "mvn compile"
                    // sh "bash runBenchmark.sh" bash script to run the tomcat webservice
                }
            }
        }
    }
}