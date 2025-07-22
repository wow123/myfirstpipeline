pipeline {
    agent any
    options {
        skipStagesAfterUnstable()
    }
    stages {
        stage('Build') {
            steps {
                echo 'Building'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing'
            }
        }
        stage('Deploy - Staging') {
            steps {
                echo 'Deploying - Staging'
            }
        }
        stage('Deploy - Production') {
            steps {
                echo 'Deploying - Production'
            }
        }
    }
}
