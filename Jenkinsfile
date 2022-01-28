pipeline {
  agent {
    docker {
      image 'node:6-alpine'
      args '-p 3000:3000'
    }

  }
  stages {
    stage('Build') {
      steps {
        sh 'npm config set proxy http://10.1.108.51:7890 ; npm config set https-proxy http://10.1.108.51:7890 ;npm install'
      }
    }

  }
}
