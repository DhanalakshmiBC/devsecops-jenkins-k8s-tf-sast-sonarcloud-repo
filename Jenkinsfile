pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=deepuorg -Dsonar.organization=deepuorg -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=8ea9f40083e0db4ab94fb64a59eb25e3ae4d8dae'
			}
        } 
  }
}
