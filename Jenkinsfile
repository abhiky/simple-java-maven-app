pipeline {
  agent {
    docker {
      image 'registry.access.redhat.com/rhel7.4:latest'
    }

  }
  stages {
    stage('googlecurl') {
      parallel {
        stage('somestage') {
          steps {
            sh 'curl -k -v https://google.com'
          }
        }
        stage('githubcurl') {
          steps {
            sh 'curl -k -v https://github.com/'
          }
        }
      }
    }
    stage('print something') {
      steps {
        echo 'hello'
      }
    }
  }
}
