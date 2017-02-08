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
        parallel node1: {
          node('master') {
            checkout scm
            sh 'ls'
            sh 'sleep 50'
            echo 'Hi 1'
            sh 'sleep 50'
            echo 'Hi 2'
          }
        }, node2_0: {
          node('master') {
            checkout scm
            sh 'ls'
            sh 'sleep 50'
            echo 'Hi 1'
            sh 'sleep 50'
            echo 'Hi 2'
          }
        }, node2_1: {
          node('master') {
            checkout scm
            sh 'ls'
            sh 'sleep 50'
            echo 'Hi 1'
            sh 'sleep 50'
            echo 'Hi 2'
          }
        }, node2_2: {
          node('master') {
            checkout scm
            sh 'ls'
            sh 'sleep 50'
            echo 'Hi 1'
            sh 'sleep 50'
            echo 'Hi 2'
          }
        }, node2_3: {
          node('master') {
            checkout scm
            sh 'ls'
            sh 'sleep 50'
            echo 'Hi 1'
            sh 'sleep 50'
            echo 'Hi 2'
          }
        }, node3: {
          node('master') {
            checkout scm
            sh 'ls'
            sh 'sleep 50'
            echo 'Hi 1'
            sh 'sleep 50'
            echo 'Hi 2'
          }
        }, failFast: false
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
