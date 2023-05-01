pipeline {
    agent any
    stages {
        stage('deploy') {
            steps {
              bash "aws configure set region $AWS_DEFAULT_REGION" 
              bash "aws configure set aws_access_key_id $AWS_ACCESS_KEY_ID"  
              bash "aws configure set aws_secret_access_key $AWS_SECRET_ACCESS_KEY"
              bash "aws s3 cp Code/index.html s3://kkt369"
            }
        }
    }
}
