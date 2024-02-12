pipeline {
agent any
stages {
    
    stage('CODE ANALYSIS-SONARQUBE') {
        steps {
           sh 'echo sonar analysis completed'
            sh 'cd webapp && sudo docker run  --rm -e SONAR_HOST_URL="http://65.1.132.50:9000" -e SONAR_LOGIN="sqp_23db14aac1a6abdbb26d03f66c2a161eef6b52ea"  -v ".:/usr/src" sonarsource/sonar-scanner-cli -Dsonar.projectKey=lms'
      }
    }

}
}
