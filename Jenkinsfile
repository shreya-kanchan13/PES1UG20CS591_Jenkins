pipeline{
  agent any
  stages{
    stage('Build){
          steps {
            sh 'cd main && g++ pipeline_591.cpp'
            echo 'Build Stage successful'
          }
          }
          stage ('Test'){
            steps{
              sh 'cd main && ./a.exe'
              eho 'Test Stage Successful'
            }
          }
          }
          post{
            failure{
              echo 'Pipeline failed'
            }
          }
         }
    
