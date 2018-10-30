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
      input {
                message "Should we continue to deplly to $THISENV ?"
                ok "Yes, we should."
                submitter "adrian,prod-dev-1,test-dev-1"
                parameters {
                    string(name: 'PERSON', defaultValue: 'Mr Jenkins', description: 'Who should I say hello to?')
                }
      }
      steps {
         sh 'echo DEPLOY TO $THISENV using the DEPLOY CREDENTIALS $DEPLOYCREDS - deliberately masked in output'
        
        
        // now do the real work ...
     
      }
    }
  }
}
