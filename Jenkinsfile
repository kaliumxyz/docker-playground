pipeline {
  agent { docker 'node:8.8' }
  stages {
    stage('build') {
      steps {
        sh 'npm -v'
      }
    }
  }
  post {
    always {
      junit 'build/reports/**/*.xml'
      sh 'echo wat'
    }
}
