pipeline {
    agent any

    stages {

        stage('Clone Code') {
            steps {
                git 'https://github.com/your-username/jenkins-app.git'
            }
        }

        stage('Install Dependencies') {
            steps {
                sh 'npm install'
            }
        }

        stage('Build') {
            steps {
                echo 'No build step needed'
            }
        }

        stage('Test') {
            steps {
                echo 'No tests added'
            }
        }

        stage('Deploy') {
            steps {
                sh '''
                pkill node || true
                nohup node app.js &
                '''
            }
        }
    }
}