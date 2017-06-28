pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        parallel(
          "build": {
            echo 'build'
            
          },
          "codereview": {
            echo 'code review'
            
          }
        )
      }
    }
    stage('qa') {
      steps {
        echo 'qa stage'
      }
    }
    stage('stage') {
      steps {
        echo 'staging'
      }
    }
  }
}