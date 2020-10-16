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

        stage('git clone success') {
            steps {
                sh "git clone success"
            }
        }

        stage('docker') {
            steps {
                container ('container'){
                sh "docker build -t python:jk8s ."
                }
            }
        }

    }

}
