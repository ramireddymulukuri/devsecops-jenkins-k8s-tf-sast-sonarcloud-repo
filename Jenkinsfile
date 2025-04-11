pipeline {
  agent any
  tools { 
        maven 'maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=ingrid -Dsonar.organization=test -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=fbddb406b214275a36b772ca5794b72369bf9949'
			}
        } 
  }
}
