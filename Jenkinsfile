@Library('shared-lib') _

pipeline {
  agent any
  stages {
   
    stage('Purge') {
      steps {
        killOldBuilds()
        echo 'Purging Running Old Builds From This PR'
      }
    }
    stage('Stage One') {
      steps {
        helloWorld()
        echo 'Stage: 1'
        sleep 15
      }
    }

    stage('Stage Two') {
      steps {
        echo 'Stage: 2'
        sleep 15
      }
    }

    stage('Stage Three') {
      steps {
        echo 'Stage: 3'
        sleep 15
      }
    }

    stage('Stage Four') {
      steps {
        echo 'Stage: 4'
        sleep 15
      }
    }

  }
  post {
        always {
            echo '## BEGIN ALWAYS BLOCK ##'
            echo 'Cleaning'
            sleep 5
            echo '## END ALWAYS BLOCK ##'
        }
   }
  environment {
    Main = '0'
  }
}
