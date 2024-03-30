pipeline {
  agent any
  stages {
    stage('check out') {
      steps {
        git(url: 'https://github.com/soumya-khanna/465a6.git', branch: 'master')
      }
    }

    stage('run') {
      steps {
        sh 'mvn verify'
      }
    }

  }
}