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
        input(message: 'Are you sure to deploy', ok: 'yes iam sure', cancel: 'no i am not ')
        echo 'deployment completed'
      }
    }

    stage('Notify for new build  ') {
      steps {
        echo 'new build completed'
      }
    }

  }
}