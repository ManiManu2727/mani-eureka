// This pipeline is for Eureka microservice deployment
pipeline {
    agent {
        label 'java-slave'
    }

    // tools section
    tools {
        maven 'maven-3.9.11'
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