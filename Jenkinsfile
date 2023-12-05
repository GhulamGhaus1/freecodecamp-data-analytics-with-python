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

        stage('new') {
          steps {
            sh 'cd FreeCodeCamp-Data-Analysis-with-Python-Course-main/ && ls -la'
          }
        }

      }
    }

  }
}