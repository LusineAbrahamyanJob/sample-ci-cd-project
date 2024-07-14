pipeline {
    agent any

    stages {
        stage("Build") {
            steps {
                echo "Building..."
                sh "python hello.py"
            }
        }
        stage("Test") {
            steps {
                echo "Testing..."
                // Add your test steps here (if any)
            }
        }
        stage("Deploy") {
            steps {
                echo "Deploying..."
                // Add your deploy steps here (if any)
            }
        }
    }
}
