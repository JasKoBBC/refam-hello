pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                sh 'cd ./lambda/custom'
                sh 'npm init'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                sh 'npm test'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}