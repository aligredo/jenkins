pipeline {
  agent any
  stages {
    stage('Stage One') {
      steps {
        echo 'Stage: 1'
        timeout(time: 15)
      }
    }

    stage('Stage Two') {
      steps {
        echo 'Stage: 2'
        timeout(time: 15)
      }
    }

    stage('Stage Three') {
      steps {
        echo 'Stage: 3'
        timeout(time: 15)
      }
    }

    stage('Stage Four') {
      steps {
        echo 'Stage: 4'
        timeout(time: 15)
      }
    }

    stage('Stage Five') {
      steps {
        echo 'Stage: 5'
        timeout(time: 15)
      }
    }

    stage('Clean') {
      steps {
        echo 'Cleaning'
        timeout(time: 5)
      }
    }

  }
  environment {
    Main = '0'
  }
}