pipeline {
  stages {
    stage('Start') {
      node('master') {
        checkout scm
        echo 'Hi'
      }
    }

    stage('Test') {
      node('master') {
          checkout scm
          sh 'sleep 10'
          echo 'Hi 1'
          sh 'sleep 10'
          echo 'Hi 2'
      }

      node('master') {
          checkout scm
          sh 'sleep 10'
          echo 'Hi 1'
          sh 'sleep 10'
          echo 'Hi 2'
      }

      node('master') {
          checkout scm
          sh 'sleep 10'
          echo 'Hi 1'
          sh 'sleep 10'
          echo 'Hi 2'
      }
    }

    stage('End') {
      node('master') {
        checkout scm
        echo 'Au revoir'
      }
    }
  }
}
