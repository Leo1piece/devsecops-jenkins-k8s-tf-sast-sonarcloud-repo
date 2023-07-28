pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {    
        sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgleotest -Dsonar.organization=asgleotest -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=6d26dc22d2c1a3996ebdd1a01b5ab979be7d1a0e'
            }
        } 
  }
}
