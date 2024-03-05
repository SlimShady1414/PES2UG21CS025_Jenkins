pipeline {
  agent any
  stages {
    stage('Bui' {
          steps {
            buid 'PES2UG21CS01'
            sh 'g++ main.cpp -o output'
          }
          }
          stage('Test') {
            steps {
              sh './output'
            }
          }
          stage('Deploy') {
            steps {
              echo 'deploy'
            }
          }
  }
  post{
    failure{
      error 'Pipeline failed'
    }
  }
}
          
