pipeline {
  agent any
  tools { 
        maven 'Maven_3_6_3'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=vbobuggywebapp -Dsonar.organization=vbobuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=c371531f45b1ce73726384eb287bebad07246fd0
			}
        } 
  }
}
