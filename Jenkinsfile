pipeline {
  stages {
    stage('Start') {
      echo 'Hi'
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

    stage('Start') {
      echo 'Au revoir'
    }
  }
}
