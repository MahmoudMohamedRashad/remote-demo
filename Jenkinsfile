pipeline{
    agent any
    stages{
        stage("build"){
            steps{
                script{
                    echo"hello from build"
                }
            }
        }
        stage("test"){
            steps{
                script{
                    echo"hello from test"
                }
            }
        }
    }
    post {
  success {
   started ${env.JOB_NAME} ${env.BUILD_NUMBER} (<${env.BUILD_URL}|Open>)
   }
  }

    }
