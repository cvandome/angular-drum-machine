pipeline {
    
    agent any
    
    stages {
        stage('Build') {
            steps {
                sh 'npm install'
                sh 'npm run build'
                sh 'npm test'
                stash name: 'dist', includes: 'dist/'
            }
        }
    }
    
}
