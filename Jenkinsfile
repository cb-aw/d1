pipeline {
  agent any
  stages {
    stage('deploy') {
       environment {
               DEPLOYCREDS = credentials('deployment-env-credentials')
            }
      steps {
         sh 'echo DEPLOY TO $THISENV using the DEPLOY CREDENTIALS $DEPLOYCREDS - deliberately masked in output'
        
        // now do the real work ...
     
      }
    }
  }
}
