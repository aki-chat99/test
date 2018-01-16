pipeline {
  agent any
  stages {
    stage('plan') {
      steps {
        echo 'current directory'
        sh '''pwd
cd /var/lib/jenkins/demo/demo
pwd
#./test.sh
whoami
echo $0'''
      }
    }
  }
}