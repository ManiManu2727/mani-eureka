// This pipeline is for Eureka microservice deployment
pipeline {
    agent {
        label 'java-slave'
    }

    // tools section
    tools {
        maven 'maven-3.9.11'
        jdk 'JDK-21.0.8'
    }
    stages {
        stage ('Build'){
            steps {
                // using mavan
                echo "********* Building Eureka Application *********"
                sh "mvn clean package"
            }
        }
    }
}