pipeline {
  agent none
  stages {
    stage('Back-end') {
      agent {
       dockerfile {
        filename 'Dockerfile.build'
        dir 'build'
        label 'static-agent'
           }
      }
      steps {
        sh 'mvn --version'
      }
    }
  }
}  
