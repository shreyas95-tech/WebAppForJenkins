pipeline {
    agent any
    tools {
        // Specify the Maven tool name as configured in Jenkins Global Tool Configuration
        maven 'maven-3.6.3'  // Use the name 'maven-3.6.3' as configured in the Global Tool Configuration
    }
    stages {
        stage('Clean and Install') {
            steps {
               // Run Maven clean install using shell command
               sh 'mvn clean install'
            }
        }
        stage('Package') {
            steps {
               // Run Maven package using shell command
               sh 'mvn package'
            }
        } 
    }
}
