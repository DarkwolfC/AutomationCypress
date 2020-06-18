pipeline {
agent any
  stages {
    stage('Init Datalake') {   
	
	stage('Data quality check') {
      steps {
        git url: 'https://github.com/DarkwolfC/AutomationCypress.git' 
        bat label: 'install npm package', script: 'npm install'
        bat label: '', script: 'dir'
        bat label: 'install cypress', script: 'npm install cypress '  
        bat label: 'valor paramentro', script: 'echo %Script%'     
        bat label: 'valor paramentro', script: 'echo %parametro%'
        bat label: 'run test', script:  'npm run %Script% echo %parametro%'
       //sh 'echo hola'
        //sh 'cypress run --browser electron --record --key 8c36a886-6113-435e-be76-54f4de49853f'
       // sh "npm run test:ci:record"
      }
    }
	
  
