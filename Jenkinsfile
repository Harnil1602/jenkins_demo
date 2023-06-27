pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout([$class: 'GitSCM',
                    branches: [[name: '*/main']],
                    doGenerateSubmoduleConfigurations: false,
                    extensions: [],
                    userRemoteConfigs: [[url: 'https://github.com/Harnil1602/jenkins_demo.git']]
                ])
            }
        }

        stage('Build') {
            steps {
                sh 'echo "Build your application here"'
                // Add commands or scripts to build your application
            }
        }

        stage('Test') {
            steps {
                sh 'echo "Run tests here"'
                // Add commands or scripts to run tests on your application
            }
        }

        stage('Deploy') {
            steps {
                sh 'scp index.html Harnil@13.232.50.20 :/var/www/html'
                // Add commands or scripts to deploy your application
            }
        }
    }
}

