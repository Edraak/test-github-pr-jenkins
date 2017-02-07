pipeline {
  stages {
    stage('Start') {
      node('master') {
        steps {
          checkout scm
          sh 'ls'
          echo 'Hi'
        }
      }
    }

    stage('Test') {
      node('master') {
        steps {
          checkout scm
          sh 'ls'
          sh 'sleep 10'
          echo 'Hi 1'
          sh 'sleep 10'
          echo 'Hi 2'
        }
      }

      node('master') {
        steps {
          checkout scm
          sh 'ls'
          sh 'sleep 10'
          echo 'Hi 1'
          sh 'sleep 10'
          echo 'Hi 2'
        }
      }

      node('master') {
        steps {
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
      node('master') {
        steps {
          checkout scm
          echo 'Au revoir'
          sh 'ls'
        }
      }
    }
  }
}
