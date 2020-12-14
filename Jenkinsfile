pipeline {
    agent any
    stages {
        stage ('Build-Maven') {
            git url: 'https://github.com/cyrille-leclerc/multi-module-maven-project'
            withMaven {
              sh "mvn clean verify"
            } // withMaven will discover the generated Maven artifacts, JUnit Surefire & FailSafe reports and FindBugs reports
        }
        stage('Build') {
            steps {
                echo "Building..."
                sh 'mvn -B -DskipTests clean package'
            }
        }
    }
}