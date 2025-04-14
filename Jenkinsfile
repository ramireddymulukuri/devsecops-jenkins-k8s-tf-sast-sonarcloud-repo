pipeline {
  agent any
  tools { 
        maven 'maven_3.2.5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=samhitha_548 -Dsonar.organization=samhitha_548 -Dsonar.host.url=https://sonarcloud.io -Dsonar.token='6ff2d0f1a03e5512cb671f2ae767ad6931926c1f'
			}
        } 
  }
}
