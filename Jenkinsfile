pipeline {
  agent any
  stages {
    stage('aaa') {
      parallel {
        stage('aaa') {
          steps {
            echo 'haha'
            sleep 3
          }
        }
        stage('ddd') {
          steps {
            echo 'aaa'
          }
        }
        stage('eee') {
          steps {
            sleep 4
          }
        }
      }
    }
    stage('bbb') {
      steps {
        sleep 3
      }
    }
    stage('ccc') {
      steps {
        bat 'dir'
      }
    }
  }
}