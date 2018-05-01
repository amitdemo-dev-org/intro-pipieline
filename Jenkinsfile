pipeline {
    agent {
        label 'jdk9'
    }
    stages {
        stage('Say Hello') {
            steps {
              echo "Hello ${params.Name}!"
              echo "${TEST_USER_USR}"
              echo "${TEST_USER_PSW}"
              sh 'java -version'
            }
        }
    
        stage('Testing') {
         
      }
      }
    
    
     
  environment {
    MY_NAME = 'AMIT'
    TEST_USER = credentials('test-user')
  }
  parameters {
    string(name: 'Name', defaultValue: 'whoever you are', description: 'Who should I say hi to?')
  }
  
  post {
    aborted {
      echo 'Why didn\'t you push my button?'
    }
  }
  
}
