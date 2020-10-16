pipeline {
  agent {
    kubernetes {
      defaultContainer 'python'
      yaml """
        apiVersion: v1
        kind: Pod
        spec:
          containers:
            - name: 'python'
              image: 'python:3-alpine'
              command:
                - cat
              tty: true
          """
    }
  }
  
    stages {
        stage('version') {
            steps {
                sh 'python -V'
            }
        }
    }
}
