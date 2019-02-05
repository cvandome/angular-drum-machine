pipeline {
    
    agent any
    
    stages {
        stage('Build') {
            steps {
                sh 'cd public/assets/ && bower install && cd ../.. && grunt build'
            }
        }
    }
    
}
