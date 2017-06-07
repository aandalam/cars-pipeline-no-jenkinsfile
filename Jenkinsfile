pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Hello'
      }
    }
    stage('Test') {
      steps {
        parallel(
          "Test": {
            echo 'Hello Test 222'
            
          },
          "Junit": {
            sh 'sh "mvn clean test"'
            
          }
        )
      }
    }
    stage('Deploy') {
      steps {
        echo 'Hello Deploy'
      }
    }
    stage('Dev') {
      steps {
        echo 'Hello Dev'
      }
    }
    stage('Staging') {
      steps {
        echo 'Hello Staging'
      }
    }
    stage('Release') {
      steps {
        echo 'hello Release'
      }
    }
    stage('Production') {
      steps {
        echo 'Hello production'
      }
    }
  }
}