pipeline {
  agent any
  stages {
    stage('Pre-Build') {
      steps {
        parallel(
          "Pre-Build": {
            echo 'Wazaa'
            
          },
          "Validate": {
            echo 'Woo'
            
          }
        )
      }
    }
    stage('Build') {
      steps {
        parallel(
          "Build": {
            echo 'This is it!'
            
          },
          "Build Sub Task 1": {
            echo 'Wazaa 2'
            
          }
        )
      }
    }
    stage('Post') {
      steps {
        echo 'This is the end'
      }
    }
  }
}