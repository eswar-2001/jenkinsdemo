pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'Building'
          }
        }

        stage('Parallel(build)') {
          steps {
            echo 'Parallel build'
          }
        }

      }
    }

    stage('Test') {
      steps {
        echo 'testing'
      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploying'
      }
    }

  }
}