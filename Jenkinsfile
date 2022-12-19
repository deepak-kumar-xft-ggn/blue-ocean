pipeline {
  agent any
  stages {
    stage('build') {
      parallel {
        stage('build') {
          steps {
            echo 'building'
          }
        }

        stage('ParallelBuild') {
          steps {
            echo 'ParallelBuild'
          }
        }

      }
    }

    stage('Test') {
      steps {
        echo 'TestingStage'
      }
    }

    stage('Deploy') {
      steps {
        echo 'DeployingStage'
      }
    }

  }
}