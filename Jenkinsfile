pipeline  {
  agent any
  stages{
    stage('Build'){
      steps {
        sh 'g++ hello.cpp -o hello_exec'
        echo 'Build Stage Successful'
      }
    }
    stage('Test'){
      steps {
        sh '/var/jenkins_home/workspace/PES2UG20CS097-1/main/hello_exec'
        echo 'Test Stage Successful'
      }
    }
  }
  post {
    failure {
      echo 'Pipeline failed'
    }
  }
}
