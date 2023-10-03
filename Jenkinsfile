pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=newasgbuggywebapp -Dsonar.organization=newasgbuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=2affe828dfa10439ca517e211e727d86b632ab82'
			}
        } 
  }
}
