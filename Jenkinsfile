pipeline {
  agent any
  stages {
    stage('code') {
      steps {
        echo 'First stage'
      }
    }

    stage('Test ') {
      parallel {
        stage('Test ') {
          steps {
            sh '''pwd 
'''
            sleep 10
          }
        }

        stage('Test') {
          steps {
            echo 'Test Complete'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'Deploying..............'
        emailext(subject: 'Testings', body: 'This mail is created by zain janjua using jenkins pepeline', from: 'rajazainjanjua333@gmail.com', to: 'zainjanjua74@gmail.com')
      }
    }

  }
}