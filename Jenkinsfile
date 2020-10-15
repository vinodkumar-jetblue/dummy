pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh './jenksins/build.sh'
        echo 'building project'
      }
    }

    stage('test') {
      steps {
        echo 'testing'
        sh './jenkins/test.sh'
      }
    }

    stage('deploy') {
      steps {
        echo 'deploying'
        sh './jenkins/deploy.sh'
      }
    }

  }
}