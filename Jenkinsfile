pipeline {
  agent any
  stages {
    stage('Plane') {
      steps {
        echo 'i want to plane my application developemt'
      }
    }

    stage('code') {
      steps {
        echo 'developement team start working on the app'
      }
    }

    stage('build') {
      steps {
        echo 'build the application'
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'testing team test the application'
          }
        }

        stage('deploy') {
          steps {
            echo 'deploy the war files'
          }
        }

        stage('release') {
          steps {
            echo 'move to release'
          }
        }

        stage('operate') {
          steps {
            echo 'test application functionality'
          }
        }

      }
    }

  }
}