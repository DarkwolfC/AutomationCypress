pipeline {
    agent any

    stages {
        stage('Install Cypress') {
            steps {
               //sh 'npm install cypress'
               sh "npm run clean"
               sh "npm run cleanCM"
               sh 'npm install cypress --save-dev'
               sh 'dir'
               sh 'npm install --save-dev mochawesome'
               sh 'npm install --save-dev mochawesome-merge'
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
                // |sed 's/\"//g'
                //sh 'npm run $script $parameter |sed  "s/\"//g"'
                sh "npm run ${script}  --parameter=$parameter"
                sh "npm run mergeCM"
                sh "npm run merge"
                sh "npm run marge"
                //sh """npm run $script $parameter |sed  's/\"//g' | sed 's/\\(.*\\) /\\1/' """
            }
        }
    }
}
