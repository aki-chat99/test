pipeline {
  agent any
  stages {
    stage('plan') {
      steps {
        echo 'current directory'
        ws(dir: '/var/lib/jenkins/demo/demo') {
          sh './test.sh'
        }
        
      }
    }
  }
}