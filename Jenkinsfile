pipeline {
      agent any
      environment {
            //Name of the environment variable to be passed to the build script
            env = "dev"
      }     

      stages {
            stage('Init') {
                  steps {
                        echo 'Hi, this is Anshul from LevelUp360'
                        echo 'We are Starting the Testing'
                  }
            }
            stage('Build') {
                  steps {
                        echo 'Building Sample Maven Project'
                  }
            }
            stage('Deploy') {
                  steps {
                        echo "Deploying in Staging Area"
                  }
            }
            stage('Deploy Production') {
                  steps {
                        echo "Deploying in Production Area"
                  }
            }
            stage('Test') {
                  steps {
                        echo 'Testing the Sample Maven Project'
                  }
            }
                  post {
                        always {
                              echo 'I am always run even if the build fails'
                        }
                  }     

                         
      }
}