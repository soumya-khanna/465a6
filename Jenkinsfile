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
  tools {
    maven 'SE465A6M'
    jdk 'SE465A6J'
  }
  environment {
    SE465A6J = 'jdk'
  }
}