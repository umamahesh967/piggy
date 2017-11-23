pipeline {
    agent any

    stages {
 
        stage('Build'){
            steps {
                sh 'printenv'
 
            }
        }
        stage('Deploy') {
            steps {
                sh 'docker-compose -f docker-compose.yml -f docker-compose.dev.yml up  -d --build --remove-orphans '
            }
        }
    }
}
