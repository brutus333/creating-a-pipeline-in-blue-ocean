pipeline {
  agent {
    docker {
      image 'node:6-alpine'
      args '-p 3000:3000 -e http_proxy=${http_proxy} -e https_proxy=${https_proxy}'
    }
    
  }
  stages {
    stage('Build') {
      steps {
        sh 'npm install'
      }
    }
  }
}
