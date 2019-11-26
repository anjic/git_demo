pipeline{
  agent any
  environment {
    APPLICATION_WORKSPACE = sh(returnStdout: true, script: 'pwd').trim()
  }
  stages{
    stage('Verify released') {
      steps{
        echo "Verify if the application version is already released"
        script {
          sh 'pwd'
          # made comment
        }
      }
    }
    stage('Create Build') {
      steps {
        echo "Compiling code"
        script {
          sh 'java -version'
        }
      }
    }
  }
}
