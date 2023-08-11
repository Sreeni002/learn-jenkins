pipeline {
  agent {
    node {
     label 'workstation'
    }
  }

  environment {
    SAMPLE_URL = "example.com"
  }
  stages {
    stage('one') {
      steps {
        sh 'echo this is a test pipeline using Jenkins'
        sh 'echo ${SAMPLE_URL}'
      }
    }
  }
  post {
   always {
     sh 'echo Post Cleanup steps'
   }
  }
}