pipeline {
  agent any
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
    stage('docker buld') {
      steps {
        emailext(subject: 'heloo', body: 'how are u', from: 'abhi.steele@gmail.com', to: 'abhi.steele@gmail.com', replyTo: 'abhi.steele@gmail.com')
      }
    }
  }
}