pipeline {
  agent any
  stages {
    stage('Stage1') {
      steps {
        echo 'step1 from stage1'
      }
    }

    stage('Stage2') {
      parallel {
        stage('Stage2') {
          steps {
            echo 'stage2 step2'
          }
        }

        stage('Stage2A') {
          steps {
            echo 'stage2A step1'
          }
        }

      }
    }

    stage('Stage3') {
      steps {
        echo 'stage3 step1'
      }
    }

    stage('Stage4') {
      steps {
        echo 'stsge4 step1'
      }
    }

  }
}