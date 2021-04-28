
pipeline {
agent any
  stages {
    stage('abc'){
      when {
        expression {
          false
        }
      }
      
      steps {
        sh "kubectl  apply -f  deploy.yml  --kubeconfig  /admin.conf"
      }
    }
  }

}
