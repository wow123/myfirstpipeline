pipeline {
    agent any
    stages {
        stage('Deploy') {
            steps {
                sh 'echo "Running flakey-deploy.sh..."'
                retry(3) {
                    sh './flakey-deploy.sh'
                }
                sh 'echo "Running health-check.sh..."'
                timeout(time: 3, unit: 'MINUTES') {
                    sh './health-check.sh'
                }
            }
        }
    }
}
