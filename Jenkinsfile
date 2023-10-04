pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=nandohoras -Dsonar.organization=nandohoras -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=19bfc15f4fe2ebb3071ec04c948de5dd4690e490'
			}
        } 
  }
}
