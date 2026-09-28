pipeline {
    agent any

    stages {
        stage('Check Files') {
            steps {
                sh 'ls -la'
                sh 'cat Dockerfile'
            }
        }

        stage('Check App') {
            steps {
                sh 'grep -n "Flask" app.py'
                sh 'cat requirements.txt'
            }
        }

        stage('Done') {
            steps {
                echo 'Pipeline from Jenkinsfile worked!'
            }
        }
    }
}
