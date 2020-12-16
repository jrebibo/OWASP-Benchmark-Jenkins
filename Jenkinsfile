pipeline {
    agent any
//     tools {
//         maven 'Maven 3.6.3'
//     }
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