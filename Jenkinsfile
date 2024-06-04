pipeline {
    agent any
    tools {
        jdk 'jdk17'
        maven 'Maven3'
    } 

    stages {
        stage('test') {
            steps {
                echo "******TEST is in Progress**************"
                sh 'mvn clean test'
            }
        }
        stage('Package') {
            steps {
                echo "############MVN Package*****************"
                sh 'mvn package'
            }
        }
    }
}
