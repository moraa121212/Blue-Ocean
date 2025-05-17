pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Build completed'
      }
    }

    stage('Test stages') {
      parallel {
        stage('Test2') {
          steps {
            echo 'running Test2'
          }
        }

        stage('Test1') {
          steps {
            echo 'reunning Test1'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'deployment completed NEW'
      }
    }

  }
}
