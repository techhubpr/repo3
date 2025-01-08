pipeline {
  agent any
  stages {
    stage('buildStage') {
      steps {
        echo 'build'
      }
    }

    stage('DevStage') {
      parallel {
        stage('DevStage') {
          steps {
            echo 'dev'
          }
        }

        stage('QAStage') {
          steps {
            echo 'QA'
          }
        }

      }
    }

    stage('ProdStage') {
      steps {
        echo 'prod'
      }
    }

  }
}