pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=patbug -Dsonar.organization=patbug -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=19effb1680d33526f5c7c9ae6c8872db4ad552a1'
			}
        } 
  }
}
