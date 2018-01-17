pipeline {
  agent any
  stages {
    stage('plan') {
      parallel {
        stage('plan') {
          steps {
            echo 'current directory'
            ws(dir: '/var/lib/jenkins/demo1') {
              sh '''pwd
'''
            }
            
          }
        }
        stage('infra build') {
          steps {
            echo 'building infra'
            sh '''./test1.sh
sleep 30s'''
          }
        }
        stage('config infra') {
          steps {
            echo 'configure infra'
            sh './test2.sh'
          }
        }
      }
    }
  }
}