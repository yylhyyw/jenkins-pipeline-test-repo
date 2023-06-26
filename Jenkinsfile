pipeline{
  agent any
  
  stages {
    stage('test') {
      parallel {
        stage('parallel step 1') {
            steps {
              sh 'cp README.md README1.md'
            }
        }
        stage('parallel step 2') {
            steps {
              sh 'cp README.md README1.md'
            }
        }
      }
    }
  }
}
