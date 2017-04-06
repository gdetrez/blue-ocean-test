pipeline {
  agent any
  stages {
    stage('Testing') {
      steps {
        parallel(
          "Testing": {
            sh 'echo "Hello world"'
            echo 'Foobar'
            
          },
          "Not testing?": {
            echo 'Stuff...'
            
          }
        )
      }
    }
    stage('After testing') {
      steps {
        echo 'xxxx'
      }
    }
  }
}