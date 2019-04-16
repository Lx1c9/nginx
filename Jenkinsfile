pipeline {
  agent {
    dockerfile {
      filename 'dockerfile'
    }

  }
  stages {
    stage('Preflight check') {
      steps {
        sh '''echo \'preflight checking\'
echo $WORKSPACE
'''
      }
    }
  }
}