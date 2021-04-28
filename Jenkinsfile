
pipeline {
agent any
  
  parameters {
   booleanParam(name: "isDeployPod" , defaultValue: true) 
  }
  stages {
    stage('abc'){
      when {
        expression {
          params.isDeployPod
        }
      }
      
      steps {
        sh "kubectl  apply -f  deploy.yml  --kubeconfig  /admin.conf"
      }
    }
  }

}
