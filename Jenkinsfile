pipeline {
  agent any
  tools { 
        maven 'maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=mavbuggywebapp -Dsonar.organization=mavbuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=a0a6dfc31b322479b91f90e98cb0880542e27e27'
			}
        } 
  }
}
