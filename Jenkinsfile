pipeline {
    agent { docker { image 'python:3.10.7-alpine' } }

    stages {
        stage('Preparing...') {
            steps {
                echo 'Preparing...'
                sh 'pip install -r requirements.txt'
            }
        }

        stage('Running...') {
            steps {
                echo 'Running..'
                sh 'python manage.py test'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}