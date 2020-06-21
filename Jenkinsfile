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
               sh "echo ${params.script}"
            }
        }
        stage('Deploy') {
            steps {
                sh 'npm run '
            }
        }
    }
}
