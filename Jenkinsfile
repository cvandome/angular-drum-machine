pipeline {
    
    agent any
    
    stages {
        stage('Build') {
            agent {
                docker {
                    image 'node:10'
                }
            }
            steps {
                sh 'npm install'
                sh 'npm run build'
                sh 'npm test'
                stash name: 'dist', includes: 'dist/'
            }
        }
    }
    
}
