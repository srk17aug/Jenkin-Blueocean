pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh '''pwd
date'''
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'teststape'
          }
        }

        stage('test par') {
          steps {
            echo 'test parte'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Build deploy'
        sleep 13
      }
    }

  }
}