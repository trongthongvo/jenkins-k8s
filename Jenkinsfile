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
                sh 'git clone success'
            }
        }

    }

}
