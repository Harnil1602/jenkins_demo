pipeline {
    agent any

    stages {
        stage('Deploy') {
            steps {
                sh 'scp index.html Harnil@:13.232.50.20/var/www/html'
            }
        }
    }
}
