pipeline {
  agent any
  stages {
    stage('plan') {
      steps {
        echo 'current directory'
        ws(dir: '/var/lib/jenkins/demo1') {
          sh '''pwd
./test1.sh
sleep 30s
./test2.sh'''
        }
        
      }
    }
  }
}