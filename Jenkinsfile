@Library('shared-lib') _

pipeline {
  agent any
  stages {
    
    stage('Purge') {
      steps {
        def purger = new purge()
        purger.purge()
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

    stage('Stage Five') {
      steps {
        echo 'Stage: 5'
        sleep 15
      }
    }

    stage('Clean') {
      steps {
        echo 'Cleaning'
        sleep 5
      }
    }

  }
  environment {
    Main = '0'
  }
}
