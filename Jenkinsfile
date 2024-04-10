pipeline {
    agent any
    
    // Define tools section
    tools {
        // Define JDK named 'Java_8'
        jdk 'Java_8'
        // Define Maven named 'Maven_3.6.3'
        maven 'Maven_3.6.3'
    }

    stages {
        stage('CompileandRunSonarAnalysis') {
            steps {
                // Execute Maven command for clean, verify, and SonarQube analysis
                sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asecurity -Dsonar.organization=asecurity -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=1a8c641b4a027d31678c511133c3f518f93c79b4'
            }
        } 
    }
}
