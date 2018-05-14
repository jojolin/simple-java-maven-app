pipeline {
  agent any
  stages {
    stage('build') {
      parallel {
        stage('build') {
          steps {
            sh 'echo "building ..."'
          }
        }
        stage('build2') {
          steps {
            sh 'echo "building 2 ..."'
          }
        }
      }
    }
    stage('test') {
      parallel {
        stage('test') {
          steps {
            sh 'echo "test ..."'
          }
        }
        stage('test2') {
          steps {
            sh 'echo "testing 2"'
          }
        }
      }
    }
  }
}