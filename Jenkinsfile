pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggywebappnew -Dsonar.organization=asgbuggywebappnew -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=8bad54e16dfbf19d6ce8bdbca014352644ffec70'
			}
        } 
  }
}
