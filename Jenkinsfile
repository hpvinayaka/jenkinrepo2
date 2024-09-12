pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Build successful'
      }
    }

    stage('Dev') {
      parallel {
        stage('Dev') {
          steps {
            echo 'Unit testing successful'
          }
        }

        stage('FuncTest') {
          steps {
            echo 'Function testing successful'
          }
        }

      }
    }

    stage('SysTest') {
      steps {
        echo 'System testing successful'
      }
    }

    stage('Release') {
      steps {
        echo 'Released to production'
      }
    }

  }
}