pipeline {
  agent any

  stages {

    stage('Prepare Artifacts') {
      steps {
        sh '''
          zip ../frontend.zip *
        '''
      }
    }

  }

}
