pipeline {
  agent any
  stages {
    stage('Lint HTML') {
      steps {
        sh 'echo \'hello\''
      }
    }

    stage('upload to aws') {
      steps {
        s3Upload 'jenkinsexercise'
      }
    }

  }
}