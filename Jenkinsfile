pipeline {
    agent any

    stages {
        stage('Commit') {
            steps {
                echo 'Code committed'
            }
        }
        stage('Build') {
            steps {
                echo 'Building the Code...'
            }
        }
        stage('Test') {
            steps {
                echo 'Regression tests running...'
                bat 'javac Hello.java'
                bat 'java Hello'
            }
        }
        stage('Report') {
            steps {
                echo 'Reporting results...'
            }
        }
    }
}
