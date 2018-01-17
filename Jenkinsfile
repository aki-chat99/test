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
            sh '''pwd
./test1.sh'''
          }
        }
        stage('config infra') {
          steps {
            echo 'config infra'
            sh '''pwd
./test2.sh'''
          }
        }
      }
    }
  }
}