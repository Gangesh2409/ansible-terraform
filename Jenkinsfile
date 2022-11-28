pipeline {
    agent any 
    stages {
        stage('SCM Checkout') {
            steps {
                git 'https://github.com/Gangesh2409/ansible-terraform.git'
            }
        }
    }
    stages {
        stage('INIT') {
            steps {
                sh "terraform init"
            }
        stage('Validate') {
            steps {
                sh "terraform validate"
            }
        stage('Plan') {
            steps {
                sh "terraform plan"
            }
        stage('Apply') {
            steps {
                sh "terraform apply -auto--approve"
            }
        }
    }

}