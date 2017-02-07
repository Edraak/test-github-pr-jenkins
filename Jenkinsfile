pipeline {
  stages {
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
}
