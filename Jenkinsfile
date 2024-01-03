pipeline {
  agent any
  stages {
    stage('build') {
      parallel {
        stage('build') {
          steps {
            sh '''pwd
date'''
          }
        }

        stage('build 1') {
          steps {
            echo 'hi bangalore'
          }
        }

      }
    }

    stage('test') {
      steps {
        sh 'echo "hello"'
      }
    }

    stage('deploy') {
      steps {
        sh 'free'
      }
    }

    stage('email') {
      steps {
        mail(subject: 'success', body: 'ocean pipeline build successfully', to: 'kirubchanni@gmail.com')
      }
    }

  }
}