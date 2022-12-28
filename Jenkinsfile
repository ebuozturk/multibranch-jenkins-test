pipeline {
    agent none
    stages {
        stage('example build') {
            agent {
                docker 'maven:3.8.6-eclipse-temurin-11'
            }
            steps {
               echo "Hello Maven"
               sh 'mvn --version'
            }
        }
        stage('Example Jdk') {
            agent { docker 'openjdk:8-jre' } 
            steps {
               echo "Hello Java"
               sh 'java -version'
            }
        }

    }
}