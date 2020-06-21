pipeline {
    agent any

    stages {
        stage('Install Cypress') {
            steps {
               sh 'npm install cypress'
            }
        }
        stage('Test') {
            steps {
               sh "echo ${params.parameter}"
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
