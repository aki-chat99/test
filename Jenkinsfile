pipeline {
  agent any
  stages {
    stage('plan ') {
      steps {
        echo 'current directory'
        sh '''cd /var/lib/jenkins/demo/demo
su - jenkins -s/bin/bash
sh test.sh

'''
      }
    }
  }
}