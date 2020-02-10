pipeline {
  agent any
  stages {
    stage('Lint HTML') {
      steps {
        sh 'echo \'hello\''
      }
    }

    stage('Upload to AWS') {
        steps {
          withAWS(region:’us-west-2’,credentials:'e98be5d2-bceb-4e81-85c6-512c3b204978') {
            s3Upload(pathStyleAccessEnabled:true, payloadSigningEnabled: true, file:’index.html’, bucket:'jenkinsexercise')
          }
        }

  }
}
