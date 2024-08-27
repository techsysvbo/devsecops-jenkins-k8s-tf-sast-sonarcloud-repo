pipeline {
  agent any
  tools { 
        maven 'Maven_3_6_3'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=vbobuggywebapp -Dsonar.organization=vbobuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=df0170cc1e7f2bee5b8f7d8a80ff0e03a485ae85
			}
        } 
  }
}
