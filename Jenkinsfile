pipeline {
    agent any
    stages {
        stage('deploy') {
            steps {
              zsh "aws configure set region $AWS_DEFAULT_REGION" 
              zsh "aws configure set aws_access_key_id $AWS_ACCESS_KEY_ID"  
              zsh "aws configure set aws_secret_access_key $AWS_SECRET_ACCESS_KEY"
              zsh "aws s3 cp Code/index.html s3://kkt369"
            }
        }
    }
}
