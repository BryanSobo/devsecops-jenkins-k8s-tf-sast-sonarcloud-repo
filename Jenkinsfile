pipeline {
  agent any
  tools { 
        maven 'maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=MaVBuggyApp -Dsonar.organization=mavbuggyapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=b2b2bfaa37d6bdbd21d99fe9a5b315a78cf05d88'
			}
        } 
  }
}
