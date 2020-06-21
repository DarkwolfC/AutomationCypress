pipeline {
    agent any

    stages {
        stage('Install Cypress') {
            steps {
               sh 'npx install cypress'
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
                sh 'npx run $script'
            }
        }
    }
}
