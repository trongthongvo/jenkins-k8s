pipeline {
  agent {
    kubernetes {
      defaultContainer 'python'
      yamlFile 'build-pod.yaml'
    }
  }
  
    stages {
        stage('version') {
            steps {
                sh 'python -V'
            }
        }

        stage('docker build') {
            steps {
                container ('docker'){
                sh '''docker build -t python:jk8s .'''
                }
            }
        }

    }

}
