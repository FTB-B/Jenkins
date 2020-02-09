pipeline {
  agent any
  stages {
    stage('Lint HTML') {
      steps {
        sh 'echo \'hello\''
        sh 'tidy -e index.html'
      }
    }

  }
}