pipeline {
    agent any

    stages {
        stage('Deploy') {
            steps {
                sh 'scp index.html Harnil@:65.2.34.109/var/www/html'
            }
        }
    }
}
