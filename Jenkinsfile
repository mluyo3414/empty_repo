pipeline {
  agent any
  stages {
    stage('Stage 1') {
      steps {
        echo 'stage 1'
      }
    }
    stage('Stage 2 a') {
      parallel {
        stage('Stage 2 a') {
          steps {
            echo 'Stage 2 a'
          }
        }
        stage('Stage 2 b') {
          steps {
            echo 'stage 2b'
          }
        }
      }
    }
  }
  environment {
    ENV_VAR1 = 'env_var1'
  }
}