pipeline {
  agent any
  stages {
    stage('Say Hello') {
      steps {
        echo "Hello ${params.Name}!"
        echo "${MYVARNAME_USR}"
        echo "${MYVARNAME_PWD}"
        sh 'java -version'
      }
    }
    stage('Deploy') {
      input {
        message 'Should we continue?'
      }
      steps {
        echo 'Continuing with deployment'
        timeout(time: 10)
      }
    }
  }
  environment {
    MY_NAME = 'Saman'
    MYVARNAME_USR = 'SAMAN'
    MYVARNAME_PWD = 'abac123'
  }
  parameters {
    string(name: 'Name', defaultValue: 'whoever you are', description: 'Who should I say hi to?')
  }
}