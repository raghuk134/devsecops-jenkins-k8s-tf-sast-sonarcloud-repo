pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=cloudraize_cloudraize -Dsonar.organization=cloudraize -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=9fac67801a99322efb7ed61096c6f4183a7e45b5'
			}
        } 
  }
}
