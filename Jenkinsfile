pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh '''pwd
cal'''
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'test'
          }
        }

        stage('test parallel') {
          steps {
            echo 'test parallel'
          }
        }

      }
    }

    stage('prod') {
      steps {
        sleep 13
        echo 'deployed to prod'
      }
    }

  }
}