pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/JhonRiv21/jenkins-demo-ci-cd.git'
            }
        }
        stage('Install dependencies') {
            steps {
                sh 'npm install'
            }
        }
        stage('Build') {
            steps {
                sh 'npm run build'
            }
        }
        stage('Test') {
            steps {
                sh 'npm test'
            }
        }
    }
}