pipeline {	
  environment {	
    registry = "kohopay/docker-test"	
    registryCredential = 'dockerHub'	
    dockerImage = ''	
  }	
  agent any	
  stages {	

    stage('Building image') {	
      steps{	
        script {	
          dockerImage = docker.build registry + ":$BUILD_NUMBER"	
        }	
      }	
    }	
    stage('Deploy Image') {	
      steps{	
        script {	
          docker.withRegistry( '', registryCredential ) {	
            dockerImage.push()	
          }	
        }	
      }	
    }
  }	
}
