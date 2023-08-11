pipeline {
  agent {
    node {
     label 'workstation'
    }
  }
  stages {
    stage('one') {
      steps {
        sh 'echo this is a test pipeline using Jenkins'
      }
    }
  }
  post {
   always {
     sh 'echo Post Cleanup steps'
   }
  }
}