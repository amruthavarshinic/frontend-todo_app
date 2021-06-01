pipeline {
  agent {
    label ('NODEJS')
  }

  stages {

    stage('Downloade Dependencies') {
      steps {
        sh '''
          npm install
        '''
      }
    }
    
    stage('Prepare Artifacts') {
      steps {
        sh '''
          zip ../frontend.zip *
        '''
      }
    }

    stage('Upload Artifact') {
      steps {
        sh '''
         curl -v -u admin:admin123 --upload-file /var/lib/jenkins/workspace/TODO_CI-Pipelines/frontend.zip http://172.31.52.12:8081/repository/frontend/frontend.zip
        '''
      }
    }
  }

}