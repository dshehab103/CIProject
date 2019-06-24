pipeline {
    agent any
    
    tools {nodejs "node"}

    stages {
         stage('dependencies') {
            steps {
                bat 'npm install'
            }
        }
        stage('Build') {
            steps {
                bat 'npm run build'
            }
        }
        stage('tests') {
            steps {
                bat 'npm run test'
            }
        }
        stage('deploy ') {
            steps {
                bat 'npm run deploy'
            }
        }
    }
}