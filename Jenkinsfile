pipeline {
  agent any
  stages {
    stage('deploy') {
       environment {
               DEPLOY-CREDS = credentials('deployment-env-credentials')
            }
      steps {
         sh 'echo DEPLOY TO $THISENV using the DEPLOY CREDENTIALS $DEPLOY-CREDS'
     
      }
    }
  }
}
