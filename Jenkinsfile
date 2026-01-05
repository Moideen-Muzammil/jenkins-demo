pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building from local Jenkinsfile'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing from local Jenkinsfile'
            }
        }
    }

    post {
        always {
            echo 'Pipeline finished webhook'
        }
    }
}

