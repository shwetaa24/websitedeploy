pipeline {
    agent any

    stages {
        stage('Clone Repository') {
            steps {
                git credentialsId: 'github-creds', url: 'https://github.com/shwetaa24/websitedeploy.git'
            }
        }
        stage('Deploy to Server') {
            steps {
                sh 'sudo cp -r * /var/www/html/'
            }
        }
    }
}
