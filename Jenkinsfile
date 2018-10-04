pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                cd ./lambda/custom
                npm init
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                npm test
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}