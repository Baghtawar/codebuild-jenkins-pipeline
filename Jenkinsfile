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
<<<<<<< HEAD
                withAWS(credentials: 'i8BwyjyDLEUh0prysOYs+cnyr2IQkaWyq9xnLMmY', region: 'ap-south-1') {
                    sh 'aws deploy create-deployment --application-name web-app --deployment-group-name web-deployment-group --github-location repository=Baghtawar/codebuild-jenkins-pipeline,commitId=${GIT_COMMIT}'
=======
                withAWS(credentials: '04f126a3-1e81-4237-adc5-a6e86b7b4b25', region: 'ap-south-1') {
                    sh 'aws deploy create-deployment --application-name web-app --deployment-group-name web-deployment-group --github-location repository=Raghavarora09/task-pipeline,commitId=${GIT_COMMIT}'
>>>>>>> 3190a49fece2acfb14ebf4339ae2216dd2279d16
                }
            }
        }
    }
}