pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'building project'
        bat 'jenkins\\build.cmd'
      }
    }

    stage('test') {
      steps {
        echo 'testing'
        bat 'jenkins/test.cmd'
      }
    }

    stage('deploy') {
      steps {
        echo 'deploying'
        input 'Deploy ?'
        bat 'jenkins/deploy.cmd'
        
      }
    }

  }
}
