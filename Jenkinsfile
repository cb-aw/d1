pipeline {
  agent any
  stages {
    stage('deploy') {
      steps {
         sh 'echo Shell $PWD' 
        // interpolated by the shell
        sh '''echo Shell $PWD'''
        // interpolated in this file by Groovy
        sh "echo Groovy $PWD"
      }
    }
  }
}
