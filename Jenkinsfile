pipeline{
    agent any
    stages{
        stage {
            steps{
                checkout scm
            }
        } 
        stage("terraform init"){
            steps{
                sh 'terraform init'
            }
        }
        stage("terraform apply"){
            steps{
                sh 'terraform apply -auto-approve'
            }
        }
    }
}
