pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sleep 10
      }
    }
    stage('Test') {
      parallel {
        stage('1-a') {
          steps {
            echo 'hello'
          }
        }
        stage('2-a') {
          steps {
            echo '2a'
          }
        }
        stage('3-a') {
          steps {
            echo '3a'
          }
        }
      }
    }
    stage('Deploy') {
      steps {
        echo 'success'
      }
    }
  }
}