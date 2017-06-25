pipeline {
  agent {
    dockerfile {
      filename 'docker-splunk'
    }
    
  }
  stages {
    stage('git pool') {
      steps {
        git(url: 'https://github.com/shevchenkoav/docker-splunk.git', branch: 'master', changelog: true)
      }
    }
  }
  environment {
    Test = ''
  }
}