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
          zip ../frontend.zip node_modules service.js
        '''
      }
    }

    stage('Upload Artifact') {
      steps {
        sh '''
         curl -v -u admin:admin123 --upload-file /home/ubuntu/workspace/TODO_CI-Pipelines/frontend.zip http://172.31.52.12:8081/repository/frontend/frontend.zip
        '''
      }
    }
  }

}