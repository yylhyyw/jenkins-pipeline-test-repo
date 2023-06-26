pipeline{
  agent any
  
  stages {
    stage('download) {
      steps {
        sh "curl -k -C - -O https://speed.hetzner.de/100MB.bin"
      }
    }
    stage('test') {
      parallel {
        stage('parallel step 1') {
            steps {
              sh "cp 100MB.bin 10.bin"
            }
        }
        stage('parallel step 2') {
            steps {
              sh "cp 100MB.bin 10.bin"
            }
        }
      }
    }
  }
}
