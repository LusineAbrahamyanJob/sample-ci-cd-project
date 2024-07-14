pipeline {
    agent any

    stages {
        stage('Setup') {
            steps {
                sh 'python -m venv venv'
                sh '. venv/bin/activate && pip install -r requirements.txt'
            }
        }
        stage('Build') {
            steps {
                sh '. venv/bin/activate && python hello.py'
            }
        }
        stage('Test') {
            steps {
                sh '. venv/bin/activate && echo "Testing..."'
                // Add your test steps here
            }
        }
        stage('Deploy') {
            steps {
                sh '. venv/bin/activate && echo "Deploying..."'
                // Add your deploy steps here
            }
        }
    }
}
