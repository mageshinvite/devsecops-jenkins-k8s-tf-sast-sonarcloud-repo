pipeline {
    agent any
    tools { 
        maven 'Maven_3_5_2'  
    }
    stages {
        stage('Compile and Run Sonar Analysis') {
            steps {	
                sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=djcliffmixwebapp -Dsonar.organization=djcliffmixwebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=f2480ae5ce4c89ca999021debbc7bc421f172219'
            }
        } 
    }
}

