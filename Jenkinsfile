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
    }

    stages {
        stage('clone git success') {
            steps {
                sh 'echo clone git success'
            }
        }
    }
}
