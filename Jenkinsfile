pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                echo 'Checking out code from GitHub...'
                checkout scm
            }
        }
        
        stage('List Files') {
            steps {
                echo 'Project files:'
                sh 'ls -la'
            }
        }
        
        stage('Validate') {
            steps {
                echo 'Validating HTML files...'
                sh 'find . -name "*.html" -type f'
            }
        }
        
        stage('Success') {
            steps {
                echo 'Build completed successfully!'
                echo 'Countdown Timer project is ready!'
            }
        }
    }
}
