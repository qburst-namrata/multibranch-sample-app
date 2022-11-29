pipeline {
  agent any
  stages {
    stage('hello') {
      steps {
        sh 'echo "Hello World"'
      }
    }
    stage('cat README'){
      when {
        branch "fix-*"
      }
      steps {
        sh '''
        cat README.md
        '''
      }
    }
  }
}
