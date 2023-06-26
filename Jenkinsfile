pipeline{
  agent any
  
  stages {
    stage('download') {
      steps {
        sh "curl -k -C - -O https://speed.hetzner.de/1GB.bin"
      }
    }
    stage('test') {
      parallel {
        stage('parallel step 1') {
            steps {
              sh "ls"
              sh "cp 1GB.bin 10.bin"
            }
        }
        stage('parallel step 2') {
            steps {
              sh "ls"
              sh "cp 1GB.bin 10.bin"
            }
        }
      }
    }
  }
}
