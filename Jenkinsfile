pipeline{
    agent any
    tools {
        terraform 'terraform'
    }
        stage('Terraform Init'){
            steps{
                sh label: '', script: 'terraform init'
            }
        }
        stage('Terraform apply'){
            steps{
                sh label: '', script: 'terraform apply --auto-approve'
            }
        }
        stage('Terraform destroy'){
            steps{
                sh label: '', script: 'terraform destroy --auto-approve'
            }
        }
    }
