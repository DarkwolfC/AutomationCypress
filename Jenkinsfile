pipeline {
    agent any

    stages {
        stage('Install Cypress') {
            steps {
               //sh 'npm install cypress'
               sh 'npm install cypress --save-dev'
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
                //sh 'npm run $script $parameter |sed  "s/\"//g"'
                sh "npm run ${script}${parameter} |sed  's/\"//g'"
                //sh """npm run $script $parameter |sed  's/\"//g' | sed 's/\\(.*\\) /\\1/' """
            }
        }
    }
}
