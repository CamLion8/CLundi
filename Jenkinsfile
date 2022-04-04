pipeline {
  agent any
  stages {
    stage('prepare') {
      steps {
        git(url: 'https://github.com/CamLion8/CLundi.git', branch: 'main')
        echo 'coucou les mouettes'
      }
    }

    stage('build') {
      steps {
        sh 'mvn clean install'
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