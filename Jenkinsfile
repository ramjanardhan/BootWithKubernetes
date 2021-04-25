pipeline {
  environment {
    registry = "janardhan54/boot-with-k8s"
    registryCredential = 'docker-details'
    dockerImage = ''
  }
  agent any
  stages {
    stage('Git Checkout') {
      steps {
               checkout scm 
            }
    }
    
    	stage('Build') { 
            steps {
                bat 'clean package -DskipTests' 
            }
        }
  }
}
