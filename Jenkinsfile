pipeline {
  agent any
  stages {
    stage('plan ') {
      steps {
        echo 'current directory'
        sh '''cd /var/lib/jenkins/demo/demo
#sh test.sh
ssh -i ankit_565881_ohio.pem ec2-user@172.16.0.42
'''
      }
    }
  }
}