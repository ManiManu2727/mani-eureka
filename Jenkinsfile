// This pipeline is for Eureka microservice deployment
pipeline {
    agent {
        label 'java-slave'
    }
    stages {
        stage ('Build'){
            steps {
                // using mavan
                sh "mvn clean package"
            }
        }
    }
}