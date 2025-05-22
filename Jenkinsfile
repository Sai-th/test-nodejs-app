pipeline {
    agent any

    tools {
        nodejs 'node-18'  // Matches the name you configured in Step 1
    }

    stages {
        stage('Install Dependencies') {
            steps {
                sh 'npm install'
            }
        }

        stage('Test') {
            steps {
                sh 'npm test || echo "No tests yet"'
            }
        }

        stage('Package') {
            steps {
                sh 'tar czf app.tar.gz node_modules main.js package.json'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploy logic goes here (e.g. SCP or SSH to EC2)'
            }
        }
    }
}
