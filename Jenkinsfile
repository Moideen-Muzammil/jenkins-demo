pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                // Checkout the main branch explicitly
                git branch: 'main', url: 'git@github.com:Moideen-Muzammil/jenkins-demo.git'
            }
        }
        stage('Build') {
            steps { sh 'echo Building project...' }
        }
        stage('Test') {
            steps { sh 'python3 hello.py' }
        }
        stage('Deploy') {
            steps { sh 'echo Deploying project...' }
        }
    }
    post {
        success { echo 'Pipeline executed successfully!' }
        failure { echo 'Pipeline failed!' }
    }
}
