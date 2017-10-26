pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'echo one'
      }
    }
  }
  post {
    always {
      junit 'build/reports/**/*.xml'
      sh 'echo two'
    }
  }
}
