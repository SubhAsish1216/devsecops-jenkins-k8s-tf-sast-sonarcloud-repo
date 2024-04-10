pipeline {
  agent any
  tools { 
        maven 'Maven_3.2.5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asecurity -Dsonar.organization=asecurity -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=1a8c641b4a027d31678c511133c3f518f93c79b4'
			}
        } 
  }
}
