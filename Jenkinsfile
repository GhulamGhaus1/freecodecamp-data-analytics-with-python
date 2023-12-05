pipeline {
  agent any
  stages {
    stage('checkout code') {
      steps {
        git(url: 'https://github.com/GhulamGhaus1/freecodecamp-data-analytics-with-python', branch: 'jenkinbranch')
      }
    }

    stage('listfiles') {
      parallel {
        stage('listfiles') {
          steps {
            sh 'ls -la'
          }
        }

        stage('') {
          steps {
            sh 'cd freecodecamp-data-analytics-with-python/ && ls -la'
          }
        }

      }
    }

  }
}