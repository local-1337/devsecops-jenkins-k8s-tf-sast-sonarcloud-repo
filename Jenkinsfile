pipeline {
  agent any
  tools { 
        maven 'Maven_3_6_3'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=host -Dsonar.organization=host -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=3fa6b2c6fb21c9d93f3e29da47606a882d095fe8'
			}
        } 
  }
}
