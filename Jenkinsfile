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
          echo sh (returnStdout: true, script: '''#!/bin/bash
          sh 'pwd'
          #sh 'chmod +x gradlew'
          
          ''')
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
