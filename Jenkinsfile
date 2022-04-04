pipeline {
  agent any
  stages {
    stage('prepare') {
      steps {
        git(url: 'https://github.com/CamLion8/CLundi.git', branch: 'main')
      }
    }

    stage('build') {
      agent any
      steps {
        echo '2'
      }
    }

    stage('test') {
      steps {
        junit 'target/surefire-reports/TEST-*.xml'
      }
    }

    stage('deploy') {
      steps {
        echo 'h'
      }
    }

  }
}