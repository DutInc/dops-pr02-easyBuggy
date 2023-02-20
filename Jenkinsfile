pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=devsecopstesting -Dsonar.organization=firstlecture -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=35b41fa3134a3dc8a0a550b736163a381124f7e8'
			}
        } 
  }
}
