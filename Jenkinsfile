pipeline {
  agent any
  stages {
    stage('Pull SCM') {
      agent any
      steps {
        bat 'echo "pull SCM"'
      }
    }

    stage('validate code') {
      parallel {
        stage('validate code') {
          agent any
          steps {
            bat 'echo "validation sucessfull"'
          }
        }

        stage('Validation 2') {
          agent any
          steps {
            bat 'echo "validation 2 sucessful"'
          }
        }

      }
    }

    stage('Deployment') {
      agent any
      steps {
        bat 'echo "Final deployment successful"'
      }
    }

  }
}