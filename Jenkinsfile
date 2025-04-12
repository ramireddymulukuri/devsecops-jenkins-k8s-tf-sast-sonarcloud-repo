pipeline {
  agent any
  tools { 
        maven 'maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=venkatatesting -Dsonar.organization=venkatatesting -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=14b679494abf8c6d24ed26b7a32e8c4cbdd1bdd9'
			}
        } 
  }
}
