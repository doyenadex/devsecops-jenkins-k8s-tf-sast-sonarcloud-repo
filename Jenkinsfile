pipeline {
  agent any
  tools { 
        maven 'Maven_3_9_11'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=adevsecopsbuggywebapp -Dsonar.organization=adevsecopsbuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=58ab51540268be0b491a6bb744b4df332b904d42'
			}
        } 
  }
}
