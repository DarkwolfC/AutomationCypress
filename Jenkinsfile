pipeline {
agent any
  stages {
    stage('Cypress') {   
	
	stage('Data quality check') {
      steps {
        git url: 'https://github.com/DarkwolfC/AutomationCypress.git' 
        bat 'npm install'
        bat 'dir'
        bat 'npm install cypress '  
        bat 'echo %Script%'     
        bat 'echo %parametro%'
        bat 'npm run %Script% echo %parametro%'
       //sh 'echo hola'
        //sh 'cypress run --browser electron --record --key 8c36a886-6113-435e-be76-54f4de49853f'
       // sh "npm run test:ci:record"
      }
    }
	
  
