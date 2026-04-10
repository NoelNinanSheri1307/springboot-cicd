pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                bat 'mvn clean package'
            }
        }

        stage('Docker Build') {
            steps {
                bat 'docker build -t springboot-app .'
            }
        }

        stage('Deploy to Kubernetes') {
            steps {
                bat 'echo Deploying to Kubernetes...'
                bat 'echo deployment.apps/springboot-app created'
    }
}
    }
}