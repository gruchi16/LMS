pipeline {
agent any
stages {
    
    stage('CODE ANALYSIS-SONARQUBE') {
        steps {
           sh 'echo sonar analysis completed'
            sh 'cd webapp && sudo docker run  --rm -e SONAR_HOST_URL="http://13.201.49.160:9000" -e SONAR_LOGIN="sqp_296dc6833dc54034a93e0a192b99f26eae74e604"  -v ".:/usr/src" sonarsource/sonar-scanner-cli -Dsonar.projectKey=lms'
      }
    }

}
}
