pipeline {
    
    agent any
    
    stages {
        stage('Build') {
            steps {
                sh 'sudo -u root npm install'
                sh 'sudo -u root npm run build'
                sh 'sudo -u root npm test'
                stash name: 'dist', includes: 'dist/'
            }
        }
    }
    
}
