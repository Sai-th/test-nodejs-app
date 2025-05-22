pipeline {
    agent any

    tools {
        nodejs 'node-18'
    }

    stages {
        stage('Install Dependencies') {
            steps {
                sh 'npm install'
            }
        }

        stage('Debug') {
            steps {
                sh 'ls -al && pwd'
            }
        }

        stage('Package') {
            steps {
                sh 'tar czf app.tar.gz node_modules index.js package.json' // adjust if needed
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploy logic goes here...'
            }
        }
    }
}
