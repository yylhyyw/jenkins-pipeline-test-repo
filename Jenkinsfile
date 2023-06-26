pipeline{
  agent any
  
  stages {
    stage('veracode') {
      parallel {
          stage('parallel step 1') {
              steps {
                veracode applicationName: 'test', createProfile: true, criticality: 'VeryHigh', deleteIncompleteScanLevel: '0', fileNamePattern: '', replacementPattern: '', sandboxName: 'test', scanExcludesPattern: '', scanIncludesPattern: '', scanName: 'test', teams: '', uploadIncludesPattern: '**/**', vid: '', vkey: ''
              }
          }
          stage('parallel step 2') {
              steps {
                veracode applicationName: 'test', createProfile: true, criticality: 'VeryHigh', deleteIncompleteScanLevel: '0', fileNamePattern: '', replacementPattern: '', sandboxName: 'test', scanExcludesPattern: '', scanIncludesPattern: '', scanName: 'test', teams: '', uploadIncludesPattern: '**/**', vid: '', vkey: ''
              }
          }
          stage('parallel step 3) {
            steps {
                veracode applicationName: 'test', createProfile: true, criticality: 'VeryHigh', deleteIncompleteScanLevel: '0', fileNamePattern: '', replacementPattern: '', sandboxName: 'test', scanExcludesPattern: '', scanIncludesPattern: '', scanName: 'test', teams: '', uploadIncludesPattern: '**/**', vid: '', vkey: ''
              }
          }
      }
    }
  }
}
