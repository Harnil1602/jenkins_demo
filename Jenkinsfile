pipeline {
    agent any

    stages {
        stage('Deploy') {
            steps {
                sh 'scp index.html user@your-remote-server:/path/to/remote/deployment'
            }
        }
    }
}
