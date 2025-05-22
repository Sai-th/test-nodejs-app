pipeline { 
    agent any

    tools {
        nodejs 'node-18' // Match the name you configured under "Global Tool Configuration"
    }

    stages {

        stage('Install Dependencies') { 
            steps { 
                sh 'npm install' 
            }
        }

        stage('Test') { 
            steps { 
                sh 'echo "testing application..."'
            }
        }

        stage("Deploy application") { 
            steps { 
                sh 'echo "deploying application..."'
            }
        }
    }
}
