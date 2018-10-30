pipeline {
  agent any
  options {
    skipDefaultCheckout true
  }
  stages {
    stage('deploy') {
       environment {
               DEPLOYCREDS = credentials('deployment-env-credentials')
            }
      // input {
      //          message "Should we continue to deploy to the $THISENV ?"
      //          submitter "adrian,prod-dev-1,test-dev-1"
                
      }
      steps {
         sh 'echo DEPLOY TO $THISENV using the DEPLOY CREDENTIALS $DEPLOYCREDS - deliberately masked in output'
        
        
        // now do the real work ...
     
      }
    }
  }
}
