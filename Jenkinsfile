pipeline{
  agent any
  
  stages {
    stage('test') {
      parallel {
        stage('parallel step 1') {
            steps {
              sh "curl -k -C - -O https://repo1.maven.org/maven2/com/veracode/vosp/api/wrappers/vosp-api-wrappers-java/23.4.11.2/vosp-api-wrappers-java-23.4.11.2.jar"
            }
        }
        stage('parallel step 2') {
            steps {
              sh "curl -k -C - -O https://repo1.maven.org/maven2/com/veracode/vosp/api/wrappers/vosp-api-wrappers-java/23.4.11.2/vosp-api-wrappers-java-23.4.11.2.jar"
            }
        }
      }
    }
  }
}
