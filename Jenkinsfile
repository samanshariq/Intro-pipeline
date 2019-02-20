pipeline {
  agent any
  stages {
    stage('Say Hello') {
      steps {
        echo "Hello ${MY_NAME}"
        echo "${MYVARNAME_USR}"
        echo "${MYVARNAME_PWD}"
        sh 'java -version'
      }
    }
  }
  environment {
    MY_NAME = 'Saman'
    MYVARNAME_USR = 'SAMAN'
    MYVARNAME_PWD = 'Shariq124!'
  }
  parameters {
    string(name: 'Name', defaultValue: 'whoever you are', description: 'Who should I say hi to?')
  }
}