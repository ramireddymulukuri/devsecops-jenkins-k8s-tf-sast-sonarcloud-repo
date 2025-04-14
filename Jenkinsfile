pipeline {
  agent any
  tools { 
        maven 'maven_3.2.5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=Devsecopstesting -Dsonar.organization=Devsecopstesting -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=e148541d355df7ca53c643d56b164f350bbec27a'
			}
        } 
  }
}
