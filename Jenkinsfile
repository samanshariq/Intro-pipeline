pipeline {
  agent {
    label 'any'
  }
  stages {
    stage('Say Hello') {
      steps {
        echo "Hello ${MY_NAME}"
        sh 'java -version'
      }
    }
  }
  environment {
    MY_NAME = 'Saman'
  }
}