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
        sh '.\\jenkins\\test.cmd'
      }
    }

    stage('deploy') {
      steps {
        echo 'deploying'
        sh '.\\jenkins\\deploy.cmd'
      }
    }

  }
}