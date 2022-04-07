pipeline {
    agent any
 
    stages {
         stage('checkout') {
             steps {
        git([url: 'https://github.com/arjunachari12/jenkins-terraform.git', branch: 'master'])

           }
              
        }
        stage('Terraform Init') {
            steps {
                sh 'terraform init'
            }
        }
         stage('Terraform Apply') {
            steps {
                sh 'terraform apply --auto-approve'
            }
        }
        
        
    }
}
