pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=awsdevsecops1_aws -Dsonar.organization=awsdevsecops1 -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=f6e90ab78048b186236b73b037b406b60e52f623'
			}
        } 
  }
}
