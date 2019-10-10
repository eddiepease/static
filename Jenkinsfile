pipeline {
  agent any 
  stages {
    stage('Upload to AWS') {
      steps {
        withAWS(credentials:'aws_static') {
            s3Upload(file:'index.html', bucket:'udacity-p3')
        }
      }
    }
  }
}
