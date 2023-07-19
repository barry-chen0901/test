pipeline {
  agent any
  stages {
    stage('build') {
      parallel {
        stage('build') {
          steps {
            sh 'date'
          }
        }

        stage('build2') {
          steps {
            sh 'echo ${date}'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        sh 'echo "deploy"'
      }
    }

  }
}