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
                echo '${params.parameter}'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
