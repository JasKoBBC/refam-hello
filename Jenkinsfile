pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                dir ('refam-hello/lambda/custom'){
                  sh 'pwd'
                  sh 'sudo npm install'
                }
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                dir ('refam-hello/lambda/custom'){
                  sh 'pwd'
                  sh 'sudo npm test'
                }
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}