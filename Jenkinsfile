pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=buggywebapp2023 -Dsonar.organization=buggywebapp2023 -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=e61ef0ca4daf9be7fed83af44337131b1d82c5a7'
			}
        } 
  }
}
