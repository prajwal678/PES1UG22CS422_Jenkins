pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'g++ task5.cpp -o task5'
        echo 'Ting has been built my man, ya see?'
        build 'PES1UG22CS422-1'
      }
    }
    stage('Test') {
      steps {
        sh './task5'
      }
    }
    stage('Deploy') {
      steps {
        echo 'Placeholder Deploy'
      }
    }
  }
  post {
    failure {
      echo 'FAILURE, this pipeline like you'
    }
  }
}
