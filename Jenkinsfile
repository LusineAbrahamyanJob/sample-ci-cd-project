pipeline {
    agent any

    stages {
        stage('Setup') {
            steps {
                // Install Python if not already installed
                sh '''
                if ! command -v python &> /dev/null
                then
                    echo "Python could not be found"
                    exit
                fi
                '''
                // Install dependencies
                sh 'pip install -r requirements.txt'
            }
        }
        stage('Build') {
            steps {
                echo 'Building...'
                sh 'python hello.py'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
                // Add your test steps here (if any)
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'
                // Add your deploy steps here (if any)
            }
        }
    }
}

