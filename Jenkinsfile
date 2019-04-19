pipeline {
  agent { dockerfile true}
  stages {
        stage(' Docker Build Test') {
            steps {
                sh 'echo 'hello world''
                sh 'uname -ar'
                
            }
        }
   }
 }
  stages {
    stage('Preflight check') {
      steps {
        smartcheckScan(imageName: 'nginx', smartcheckHost: '192.168.1.130', smartcheckUser: 'administrator', smartcheckPassword: 'Apple1995!', findingsThreshold: '50', preregistryHost: 'gcr.io', preregistryPassword: 'c7aa79d9fa50484832a01facd4b9562f8cc9acb6', preregistryScan: true, preregistryUser: 'lcregistryadmin@river-howl-232417.iam.gserviceaccount.com', smartCheckHost: '192.168.1.130', debug: true)
      }
    }
  }
}
