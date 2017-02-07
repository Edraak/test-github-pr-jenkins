pipeline {
  agent any

  stages {
    stage('Start') {
      steps {
        node('master') {
          checkout scm
          sh 'ls'
          echo 'Hi'
        }
      }
    }

    stage('Test') {
      steps {
        node('master') {
          checkout scm
          sh 'ls'
          sh 'sleep 10'
          echo 'Hi 1'
          sh 'sleep 10'
          echo 'Hi 2'
        }

        node('master') {
          checkout scm
          sh 'ls'
          sh 'sleep 10'
          echo 'Hi 1'
          sh 'sleep 10'
          echo 'Hi 2'
        }

        node('master') {
          checkout scm
          sh 'ls'
          sh 'sleep 10'
          echo 'Hi 1'
          sh 'sleep 10'
          echo 'Hi 2'
        }
      }
    }

    stage('End') {
      steps {
        node('master') {
          checkout scm
          echo 'Au revoir'
          sh 'ls'
        }
      }
    }
  }
}
