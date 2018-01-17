pipeline {
  agent any
  stages {
    stage('plan') {
      steps {
        echo 'current directory'
        ws(dir: '/var/lib/jenkins/demo1') {
          sh '''pwd
ls -l
./test.sh
whoami
sleep 10s
pwd
./test1.sh
whoami
sleep 30s
./test2.sh'''
        }
        
      }
    }
  }
}