pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=cloudraize_cloudraize -Dsonar.organization=cloudraize -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=7ba58dac6884425b4dd268e6db57371d750b3850'
			}
        } 
  }
}
