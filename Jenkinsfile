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
        sh '''
            python3 -m venv venv
            . venv/bin/activate
            pip install --upgrade pip --no-cache-dir
            pip install flask --no-cache-dir
        '''
    }
}

        stage('Run Tests') {
            steps {
                echo 'No tests yet, skipping...'
            }
        }
        stage('Test Flask') {
    steps {
        sh '''
            . venv/bin/activate
            python3 -c "import flask; print('Flask is installed correctly')"
        '''
    }
}



        stage('Deploy') {
            steps {
                echo 'Deployment steps go here'
            }
        }
    }
}
