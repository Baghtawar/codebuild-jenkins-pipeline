pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }
        
        stage('Deploy to AWS') {
            steps {
                withAWS(credentials: 'aws-cred', region: 'ap-south-1') {
                    sh 'aws deploy create-deployment --application-name web-app --deployment-group-name web-deployment-group --github-location repository=Baghtawar/codebuild-jenkins-pipeline,commitId=${GIT_COMMIT}'
                }
            }
        }
    }
}