pipeline {
    agent any
    
    tools {
        terraform 'terraform'
    }

    stages {
         stage('checkout') {
            steps {
                git 'https://github.com/arjunachari12/jenkins-terraform'
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
