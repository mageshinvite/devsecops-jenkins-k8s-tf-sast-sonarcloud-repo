pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=webbuggyapp -Dsonar.organization=webbuggyapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=69d02c970c30a2ffd80dd721b06b72e6bab68eb0'
			}
        } 
  }
}
