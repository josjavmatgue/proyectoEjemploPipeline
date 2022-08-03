pipeline {

    agent any

    stages{

         stage('docker build'){

          steps{

             script{

                sh "docker build -f . -t  304410717/myDemo:v1-${BUILD_ID} ."
             }
         }
      }

        stage('docker push'){
          steps{
                script{
                   sh "docker push 304410717/mydemo:v1-${BUILD-ID}"
               }
          }
        }
    }
}
