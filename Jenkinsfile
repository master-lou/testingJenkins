pipeline {

  agent any

  stages {
    stage("build") {
      steps {
        echo 'Building the application...'
      }
    }
    stage("test")
    {
      steps {
        echo 'Testing the application...'
      }
    }
    stage("deploy")
    {
      steps {
        echo 'deploying the application..'
      }
    }
  }
  post {
    always {
      echo 'always runs regardless of successful or failed build'
    }
    failure {
      echo 'this only runs on failed'
    }
    success {
      echo 'this runs on success'
    }
  }


}
