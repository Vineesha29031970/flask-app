pipeline {
    agent any

    stages {
        stage('Pull Code') {
            steps {
                git branch: 'main', url: 'https:/Vineesha29031970/github.com/flask-app.git'
            }
        }

        stage('Install Dependencies') {
            steps {
                sh 'python3 -m venv venv'
                sh '. venv/bin/activate && pip install --upgrade pip && pip install flask'
            }
        }

        stage('Run Tests') {
            steps {
                echo 'No tests yet, skipping...'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deployment steps go here'
            }
        }
    }
}
