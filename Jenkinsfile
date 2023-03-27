pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=buggywebapp -Dsonar.organization=kyndryl -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=b14f80f41b614ef04bc33cb87367d01951de006b'
			}
        } 
  }
}
