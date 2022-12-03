pipeline {
  agent any
  stages {
    stage('master') {
      parallel {
        stage('master') {
          steps {
            sh '''echo \'hello from Jenkins\'
'''
          }
        }

        stage('stage1') {
          steps {
            sh '''echo \'hello from stage1\'
sleep 10'''
          }
        }

      }
    }

    stage('compile') {
      steps {
        sh '''echo \'this is compile process\'
sleep 10
'''
      }
    }

    stage('test') {
      steps {
        sh '''echo \'hi this is testing area\'
sleep 10'''
      }
    }

    stage('deploy') {
      steps {
        sh '''echo \'deploy area\'
sleep 10
'''
      }
    }

  }
}