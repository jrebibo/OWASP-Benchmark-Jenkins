pipeline {
    agent any
    tool name: 'Maven 3.6.3', type: 'maven'
//     tools {
//         maven 'Maven 3.6.3'
//     }
    stages {
        stage('Build') {
            steps {

                echo "Building..."
                sh 'mvn -B -DskipTests clean package'
                sh "mvn clean verify"
            }
        }
    }
}