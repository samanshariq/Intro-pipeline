pipeline {
  agent any
  stages {
    stage('Say Hello') {
      steps {
        echo 'Hello World'
        sh 'java -version'
      }
    }
    stage('Label') {
      steps {
        node(label: 'jdk10')
      }
    }
  }
}