pipeline {
  agent any
  stages {
    stage('m') {
      parallel {
        stage('error') {
          steps {
            sh 'echo "shell hello world"'
            sh 'echo "shell hello world"'
          }
        }

        stage('1') {
          steps {
            sh 'echo "shell hello world2"'
          }
        }

        stage('2') {
          steps {
            node(label: 'hehe') {
              sh 'echo "1"'
            }

            sh 'echo "2"'
          }
        }

      }
    }

  }
}