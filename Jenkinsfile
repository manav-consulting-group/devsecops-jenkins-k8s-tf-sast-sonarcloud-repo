pipeline {
  agent any
  tools { 
        maven 'maven'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=kobibuggywebapp -Dsonar.organization=kobibuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=54532215d4dae7144f225922f017eb5976007020'
			}
        } 
  }
}
