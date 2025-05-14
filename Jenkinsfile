pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=shivamsecuitywebapp -Dsonar.organization=shivamsecuitywebapp 
		    -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=7219856d63830bab52f19401ea2b6fbb5afc2e9f'
			}
        } 
  }
}
