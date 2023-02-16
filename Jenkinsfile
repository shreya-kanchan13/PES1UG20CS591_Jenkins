pipeline{
  agent any
  stages {
    stage('Build'){
          steps {
            sh 'cd main && g++ -o a pipeline_591.cpp'
            echo 'Build Stage successful'
          }
       }
          stage ('Test') {
            steps {
              sh  'cd main && ./a'
              echo 'Test Stage Successful'
            }
          }
          }
  post {
            failure{
              echo 'Pipeline failed'
            }
          }
         }
    
