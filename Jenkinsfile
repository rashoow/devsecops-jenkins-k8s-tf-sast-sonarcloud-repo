pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=radevwebapp -Dsonar.organization=radevwebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=b583b67e7dcf10b579ff33fd15efc5b12d2cdcaa'
			}
        } 
  }
}
