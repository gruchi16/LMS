pipeline {
    agent {
    node {
        label 'docker'
         }
        }
    environment {
    dockerhub=credentials('dockerhubuser')
    }

    stages{
    stage('CODE ANALYSIS-SONARQUBE') {
        steps {
           sh 'echo sonar analysis completed'
            sh 'cd webapp && sudo docker run  --rm -e SONAR_HOST_URL="http://13.126.89.226:9000" -e SONAR_LOGIN="sqp_2275b771b5c169421c61aa3884f8caf65d0e267f"  -v ".:/usr/src" sonarsource/sonar-scanner-cli -Dsonar.projectKey=lms'
      }
    }

}
}
