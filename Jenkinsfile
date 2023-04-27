pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asecurgurubuggywebapp -Dsonar.organization=gitlabdevsecopsci -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=47c40c99a42c0de98747ff17456d27053fd1d4c8'
			}
        } 
  }
}
