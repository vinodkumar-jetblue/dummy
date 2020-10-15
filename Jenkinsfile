pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh '''./jenkins/build.cmd
'''
        echo 'building project'
      }
    }

    stage('test') {
      steps {
        echo 'testing'
        sh './jenkins/test.cmd'
      }
    }

    stage('deploy') {
      steps {
        echo 'deploying'
        sh './jenkins/deploy.cmd'
      }
    }

  }
}