pipeline {
  
  agent any  
  
  stages {
    stage('checkout') {
      steps {
        checkout scm
  	    }
    	}
    
 
    stage('terraform plan') {
      steps {
	      sh 'terraform init'
	    sh 'terraform destroy --auto-approve'
      }
    }

  }
  
  
}
