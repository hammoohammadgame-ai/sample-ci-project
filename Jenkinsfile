pipeline {

    agent any

    stages {

        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/hammoohammadgame-ai/sample-ci-project.git'
            }
        }

        stage('Build') {
            steps {
                sh 'bash app.sh'
            }
        }

        stage('Test') {
            steps {
                sh 'bash test.sh'
            }
        }

        stage('Notify') {
            steps {
                echo 'Pipeline Executed Successfully'
            }
        }
    }
}
