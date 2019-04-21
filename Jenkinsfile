pipeline {
  agent any
  stages {
    stage('Prep') {
      parallel {
        stage('Prep') {
          steps {
            sh '''echo \'prep - 1\'
echo \'prep - 2\''''
            echo 'print message'
          }
        }
        stage('prep - others') {
          steps {
            sleep 60
          }
        }
      }
    }
    stage('finish') {
      steps {
        sh 'echo \'finish\''
      }
    }
  }
}