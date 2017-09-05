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
          "Junit": {
            echo 'Hello Junit'
            
          },
          "DBUunit": {
            sh 'sh "mvn clean test"'
            
          }
        )
      }
    }
    stage('Deploy') {
      steps {
        echo 'Hello Deploy'
        sh 'mvn clean install'
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