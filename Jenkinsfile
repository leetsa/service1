pipeline {
  agent any
  stages {
    stage('GIT') {
      steps {
        git(url: 'https://github.com/leegroup1/service.git', branch: 'feature')
      }
    }

    stage('Merge') {
      steps {
        sh '''git checkout dev
git merge feature'''
      }
    }

  }
}