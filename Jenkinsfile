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
ls -l
./test.sh'''
            }
            
          }
        }
        stage('build infra') {
          steps {
            echo 'build infra'
            ws(dir: '/var/lib/jenkins/demo1') {
              sh 'pwd'
            }
            
          }
        }
        stage('config infra') {
          steps {
            echo 'config infra'
            ws(dir: '/var/lib/jenkins/test2/chef') {
              sh 'pwd'
            }
            
          }
        }
      }
    }
  }
}