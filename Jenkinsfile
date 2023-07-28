pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {    
        sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggywebappleo -Dsonar.organization=asgbuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=62a15a0ff443fd62b3b49b8ddc21b411b70ff0f5'
            }
        } 
  }
}
